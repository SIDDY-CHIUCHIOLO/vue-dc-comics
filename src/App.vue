<template>
  <div id="app">

    <!-- header -->
    <Header />
    <!-- main -->
    <main>
      <Products />
    </main>
    <!-- footer -->
    <Footer />

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Products from './components/Products.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Products,
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
