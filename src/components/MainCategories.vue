<template>
  <div class="main-categories">
        <div class="section">
            <div class="container">
                <div v-for="(el, i) in cards" :key="i" class="col">
                    <img :src="el.image">
                    <span>{{el.text}}</span>
                </div>
            </div>
        </div>
  </div>
</template>

<script>
export default {
    name: 'Main',
    data() {
        return {
            cards: [
                {
                    image: require('../img/buy-comics-digital-comics.png'),
                    text: 'DIGITAL COMICS'
                },
                {
                    image: require('../img/buy-comics-merchandise.png'),
                    text: 'DC MERCHANDISE'
                },
                {
                    image: require('../img/buy-comics-subscriptions.png'),
                    text: 'SUBSCRIPTION'
                },
                {
                    image: require('../img/buy-comics-shop-locator.png'),
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    image: require('../img/buy-dc-power-visa.svg'),
                    text: 'DC POWER VISA'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>


    .section {
        background-color: rgb(20, 141, 255);

        .container {
            display: flex;

            .col {
                display: flex;
                width: 20%;
                gap: 10px;
                justify-content: center;
                align-items: center;

                img {
                    max-width: 30px;
                }

                span {
                    font-size: 14px;
                }
            }

        }
    }

</style>