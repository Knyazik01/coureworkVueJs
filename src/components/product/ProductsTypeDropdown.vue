<template>
  <div class="product">
    <div class="row product__controls">

      <!--            <label for="product_types" class="label_text">Choose product type:</label>-->
      <!--            <select name="type" id="product_types">-->
      <!--                <option value="most_common" class="product_type" disabled> 10 most common words (in process)</option>-->
      <!--                <option value="rarest" class="product_type">10 rarest words</option>-->
      <!--                <option value="type3" class="product_type" >Find text in sentence (in process)</option>-->
      <!--                <option value="type4" class="product_type" disabled>Type4 (in process)</option>-->
      <!--                <option value="type5" class="product_type" disabled>Type5 (in process)</option>-->
      <!--                <option value="type6" class="product_type" disabled>Type6 (in process)</option>-->
      <!--                <option value="type7" class="product_type" disabled>Type7 (in process)</option>-->
      <!--            </select>-->

      <div class="col-sm-12 col-md-6 col-lg-4 col-xl-3 dropdown">
        <a class="btn dropdown-toggle product_types" href="#" role="button" id="dropdownMenuLink"
           data-toggle="dropdown" aria-haspopup="true" aria-expanded="true">
          Choose product type:
        </a>

        <div class="dropdown-menu dropdown-menu-left dropdown-menu-lg-right" aria-labelledby="dropdownMenuLink" data-bar-is="close">
          <div class="dropdown-header">Choose product type</div>
          <!--                    <a class="dropdown-item product_type disabled" href="#">10 most common words</a>-->
          <!--                    <div class="dropdown-divider"></div>-->
          <a class="dropdown-item product_type " href="#" data-type="ten-rarest-words">10 rarest words</a>
          <div class="dropdown-divider"></div>
          <a class="dropdown-item product_type active" href="#" data-type="ten-most-common-words">10 most common words</a>
          <div class="dropdown-divider"></div>
          <a class="dropdown-item product_type disabled" href="#" data-type="type4">Type4</a>
          <div class="dropdown-divider"></div>
          <a class="dropdown-item product_type disabled" href="#" data-type="type5">Type5</a>
          <div class="dropdown-divider"></div>
          <a class="dropdown-item product_type disabled" href="#" data-type="type6">Type6</a>
          <div class="dropdown-divider"></div>
          <a class="dropdown-item product_type disabled" href="#" data-type="type7">Type7</a>
        </div>
      </div>

      <div class="col find">
        <input type="button" value="Find" id="findBtn" class="btn">
      </div>
    </div>





  </div>
</template>

<script>
export default {
  name: "ProductsTypeDropdown.vue"
}
</script>

<style scoped>

.product {
  display: flex;
  flex-direction: column;
}

.product__controls {
  margin: 20px 0;
}

.product_types, #findBtn {
  background-color: #008CBA;
  color: white;
  padding: 0.5em 1.5em;
  font-size: 1.2em;
  transition-duration: 0.4s;
  margin-top: 10px;
}

.product_types {
  padding: 0.5em 1em;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.product_types:hover, #findBtn:hover, .btnClicked {
  background-color: white;
  color: black;
}

.product_type {
  font-size: 1em;
  display: block;
}

.dropdown-menu {
  margin: 5px 15px 0 15px;
  /*display: block;*/
  width: calc(100% - 30px);
  /*background-color: #00a9e2;*/
}

.product_type {
  padding: 0.5rem 1.5rem;
}

.product_type:hover {
  background-color: #00a9e2;
  color: #fff;
}



</style>