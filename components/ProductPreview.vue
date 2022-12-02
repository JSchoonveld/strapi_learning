<template>
  <div class="flex flex-col">
    <h1 class="text-3xl font-bold">
      {{ product.attributes.name }}
    </h1>
    <span>
    {{ product.attributes.price }}
  </span>
    <NuxtLink :to="`/products/${product.id}`">Read more</NuxtLink>
  </div>
</template>

<script>
export default {
  props: ['product']
}
</script>