<template>
  <div id="app">

    <!-- header -->
    <Header />
    <!-- main -->
    <Main />
    <!-- footer -->
    <Footer />

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "./assets/SCSS/style.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
