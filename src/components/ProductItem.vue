<template>
  <div class="card text-left mb-3 mx-3">
    <img class="card-img-top" :src="imageUrl" alt="Product Image">

    <div class="card-body">
      <h4 class="card-title height-3">{{ product.name }}</h4>
      <p class="card-text text-danger">{{ product.price }} VND</p>
    </div>

    <div class="d-flex justify-content-center mb-2">
      <button class="btn btn-danger mr-2">Buy</button>
      <button class="btn btn-primary">Detail</button>
    </div>
  </div>
</template>
<script>
export default {
  name: "ProductItem",
  props: {
    product: {
      type: Object,
      required: true,
    }
  },
  computed: {
    imageUrl() {
      return require(`@/assets/images/${this.product.image}.webp`);
    }
  }
}
</script>
<style scoped></style>