<script setup lang="ts">
const { capital, img, name, population, region } = defineProps<{
  name: string
  population: string
  region: string
  capital: string
  img: string
}>()
</script>
<template>
  <article>
    <figure>
      <img :src="img" :alt="name" />
    </figure>
    <div>
      <p>Population: {{ population }}</p>
      <p>Region: {{ region }}</p>
      <p>Capital: {{ capital }}</p>
    </div>
  </article>
</template>
