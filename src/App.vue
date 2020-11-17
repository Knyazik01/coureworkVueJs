<template>
  <div id="app">
    <main class="main">
      <!--    <Header />-->
      <ProductsTypeDropdown
          @sendType="fetchProductType"
      />
      <butFind
          :product-type="this.type"
          :input-data="this.inpText"
          @sendResult="fetchResult"
      />
      <!--    <div class="inputs"></div>-->
      <Inputs
          @sendInput="fetchInput"
          :result-data="this.type"
      />
      <Footer/>
    </main>


    <!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
// import Header from "@/components/header/Header";
import ProductsTypeDropdown from "@/components/product/ProductsTypeDropdown";
import butFind from "@/components/product/butFind";
import Inputs from "@/components/input/Inputs";
import Footer from "@/components/footer/Footer";

export default {
  name: 'App',
  data: () => ({
    type: '',
    inpText: '',
    resText: '',
  }),
  components: {
    // HelloWorld,
    // Header,
    ProductsTypeDropdown,
    butFind,
    Inputs,
    Footer
  },
  methods: {
    fetchProductType(type) {
      this.type = type;
      console.log(type);
    },

    fetchInput(text) {
      this.inpText = text;
      console.log('inp', text);
    },

    fetchResult(text) {
      this.resText = text;
      console.log('res', text);
    },
  },

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
  width: 95%;
  padding: 10px;
  display: flex;
  flex-direction: column;
}

</style>
