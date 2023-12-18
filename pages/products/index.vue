<template>
  <div class="container">
    <div class="list">
      <div v-for="product in products" :key="product.id">
        <ProductCard :product="product" />
      </div>
    </div>
  </div>
</template>

<script setup>
  useHead({
    title: 'Nuxt Shop | Produtos'
  })
  const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<style scoped>
  .list {
    display: flex;
    flex-wrap: wrap;
  }
</style>