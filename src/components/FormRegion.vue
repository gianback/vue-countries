<script setup lang="ts">
import { ref } from 'vue'

const regions = ref(['Antarctic', 'Americas', 'Europe', 'Africa', 'Asia', 'Oceania'])
</script>

<template>
  <form>
    <div class="relative shadow-lg max-w-[200px]">
      <select
        class="pl-4 pr-10 py-3 w-full rounded-md bg-transparent appearance-none"
        name="region"
        id="region"
      >
        <option class="px-4 py-3" v-for="region in regions" :value="region" :key="region">
          {{ region }}
        </option>
      </select>
      <i class="pi pi-angle-down absolute right-6 top-1/2 -translate-y-1/2 text-xl"></i>
    </div>
  </form>
</template>
