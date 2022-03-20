<template>
  <div id="app">
    <Header />
    <MainWrapper/>
    <MainCategories />
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainWrapper from './components/MainWrapper.vue'
import MainCategories from './components/MainCategories.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    MainWrapper,
    MainCategories,
    Footer    
  }
}
</script>

<style lang="scss">
#app {
  height: 100vh;
  width: 100vw;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: white;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  max-width: 1024px;
  margin: 0 auto;
  padding: 30px 0;
}

ul {
  padding: 0;

  li {
  list-style: none;
  }
}

a {
  cursor: pointer;
  text-decoration: none;
  color: white;
}

</style>
