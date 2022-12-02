<template>
  <div
      class="min-h-[500px] relative flex items-end justify-center my-6 rounded-[5px] overflow-hidden"
  >
    <div
        class="relative z-10 w-full text-center bg-gradient-to-t from-black/70 via-black/50 to-transparent py-6"
    >
      <h1 class="text-6xl text-white font-bold mb-3">
        {{ hero.headline }}
      </h1>
      <h2 class="text-4xl text-white font-light">
        {{ hero.subheadline }}
      </h2>
    </div>
    <img
        :src="hero.background_image.filename"
        :alt="hero.background_image.alt"
        class="absolute top-0 left-0 z-0 w-full h-full object-cover"
    />
  </div>
</template>

<script>
export default {
  props: ['hero']
}
</script>