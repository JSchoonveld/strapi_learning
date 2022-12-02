<script setup>

const route = useRoute();
const { data: product} = await useFetch(`http://localhost:1337/api/products/${route.params.id}`);
</script>

<template>
  <h1 class="text-3xl font-bold">
    {{ product.data.attributes.name}}
  </h1>
  <NuxtLink to="/products">Back</NuxtLink>
</template>

<script>
export default {
  props: ['']

}
</script>