<template>
  <div class="footer">
      <div class="first-section">
          <div class="container">
              <div class="col">
                  <div class="nav-col">
                      <h3>DC COMICS</h3>
                      <span>Characters</span>
                      <span>Comics</span>
                      <span>Movies</span>
                      <span>TV</span>
                      <span>Games</span>
                      <span>Videos</span>
                      <span>News</span>
                  </div>
                  <div class="nav-col">
                      <h3>SHOP</h3>
                      <span>Shop DC</span>
                      <span>Shop DC Collectives</span>
                  </div>
              </div>
              <div class="col">
                  <div class="nav-col">
                      <h3>DC</h3>
                      <span>Terms of Use</span>
                      <span>Privacy Policy</span>
                      <span>Ad Choices</span>
                      <span>Advertising</span>
                      <span>Jobs</span>
                      <span>Subscriptions</span>
                      <span>Talent Workshops</span>
                      <span>CPSC Certificates</span>
                      <span>Ratings</span>
                      <span>Shop Help</span>
                      <span>Contact Us</span>
                  </div>
              </div>
              <div class="col">
                  <div class="nav-col">
                      <h3>SITES</h3>
                      <span>DC</span>
                      <span>MAD Magazine</span>
                      <span>DC Kids</span>
                      <span>DC Universe</span>
                      <span>DC Power Visa</span>
                  </div>
              </div>
          </div>
      </div>
      <div class="second-section">
          <div class="container">
              <div class="button">
                  SIGN-UP NOW!
              </div>
              <div class="social">
                  <div class="follow">
                      FOLLOW US
                  </div>
                  <div class="list-social">
                      <a href="#">
                          <img src="../img/footer-facebook.png" alt="">
                      </a>
                      <a href="#">
                          <img src="../img/footer-twitter.png" alt="">
                      </a>
                      <a href="#">
                          <img src="../img/footer-youtube.png" alt="">
                      </a>
                      <a href="#">
                          <img src="../img/footer-pinterest.png" alt="">
                      </a>
                      <a href="#">
                          <img src="../img/footer-periscope.png" alt="">
                      </a>
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss" scoped>



    .first-section {
        background-image: url('../img/footer-bg.jpg');

        .container {
            display: flex;
            gap: 30px;

            .col {
                display: flex;
                flex-direction: column;
                gap: 20px;

                .nav-col {
                    display: flex;
                    flex-direction: column;
                    gap: 5px;

                    h3 {
                        margin: 0 0 7px;
                    }
                }
            }
            
        }
        
    }

    .second-section {
        background-color: rgb(58, 56, 56);

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;

            .button {
                border: 2px solid rgb(20, 141, 255);
                padding: 10px;
                cursor: pointer;
            }

            .social {
                display: flex;
                align-items: center;
                gap: 20px;

                .list-social {
                    display: flex;
                    gap: 10px;

                }
            }
        }
    }

</style>