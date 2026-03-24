<template>
  <section class="product-list">
    <h2 class="text-center text-danger font-weight-bold">List of highlight products</h2>
    <div class="product-list row">
      <div class="col-lg-3" v-for="product of products" :key="product.id">
        <ProductItem :product="product" />
      </div>
    </div>
  </section>
</template>
<script>
import products from "@/assets/data/productList.json";
import ProductItem from "./ProductItem.vue";

export default {
  name: "ProductList",
  components: {
    ProductItem
  },
  data() {
    return {
      products
    };
  }
}
</script>
<style scoped></style>