<template>
  <div id="app">
    <main class="main">
      <!--    <Header />-->
      <!--    <ProductsTypeDropdown />-->
      <!--    <butFind />-->
      <!--    <div class="inputs"></div>-->
      <Footer />
    </main>


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

  background-color: #000;
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

.main {
  width: 90%;
  display: flex;
  flex-direction: column;
  margin: 0 40px;
}
</style>
