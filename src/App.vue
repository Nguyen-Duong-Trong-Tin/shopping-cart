<template>
  <TheHeader />

  <main>
    <ProductList />
  </main>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import ProductList from './components/ProductList.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    ProductList
  }
}
</script>

<style></style>
