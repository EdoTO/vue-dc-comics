<template>
  
  <div class="header">
    <div class="container">
      <img class="logo" src="../img/dc-logo.png" alt="">
      <div class="navbar">
        <ul>
          <li v-for="(el, i) in links" :key="i"  class="nav-item">
            <a href="#" >{{ el.text }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>

</template>

<script>
export default {
    name: 'Header',
    data () {
      return {
        links: [
          {
            text: 'CHARACTERS',
            href: 'https://www.google.com'
          },
          {
            text: 'COMICS',
            href: 'https://www.google.com'
          },
          {
            text: 'MOVIES',
            href: 'https://www.google.com'
          },
          {
            text: 'TV',
            href: 'https://www.google.com'
          },
          {
            text: 'GAMES',
            href: 'https://www.google.com'
          },
          {
            text: 'COLLECTIBLES',
            href: 'https://www.google.com'
          },
          {
            text: 'VIDEOS',
            href: 'https://www.google.com'
          },
          {
            text: 'FANS',
            href: 'https://www.google.com'
          }
        ]
      }
    }
}
</script>

<style lang='scss' scoped>

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 0 20px;

  .logo {
    width: 100px;
  }

  .navbar ul {
    display: flex;

    .nav-item {
      padding: 10px;
      font-size: 14px;
      
      a {
        color: black;
      }

      &.active, &:hover {
        a::after {
          content:'';
          display: block;
          height: 3px;
          position: absolute;
          left: 0;
          right: 0;
          bottom: 0;
          background-color: rgb(20, 141, 255);
        }
      }
    }
  }
}

</style>