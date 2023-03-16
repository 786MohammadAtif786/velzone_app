<template>
  <Product />
  <ProductGallery />
  <GeneralInfo />
  <Button />

</template>

<script>
import Product from './components/Product.vue'
import ProductGallery from './components/ProductGallery.vue';
import GeneralInfo from './components/GeneralInfo.vue'
import Button from './components/Button.vue';

export default {
  name: 'App',
  components: {
    Product,
    ProductGallery,
    GeneralInfo,
    Button
  }
}
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #060708;
  margin-top: 10px;
} */
.main-container {
        max-width: 900px;
        margin: 30px auto;
        background: rgb(253, 251, 251);
        text-align: left;
        padding: 40px;
        border-radius: 10px;
    }
</style>
