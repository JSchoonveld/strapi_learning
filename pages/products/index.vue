<template>
  <h1 class="text-3xl font-bold">
    Products
  </h1>
  <ProductPreview v-for="product in products.data" :product="product" :key="product.id"/>
</template>

<script setup>
const {data: products} = await useFetch('http://localhost:1337/api/products');
</script>