<template>
  <div id="app">
<!--    <Header />-->
<!--    <ProductsTypeDropdown />-->
<!--    <butFind />-->
<!--    <div class="inputs"></div>-->
    <Footer />

<!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
// import Header from "@/components/header/Header";
// import ProductsTypeDropdown from "@/components/product/ProductsTypeDropdown";
// import butFind from "@/components/product/butFind";
import Footer from "@/components/footer/Footer";

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Header,
    // ProductsTypeDropdown,
    // butFind,
    Footer
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #000;
}
</style>
