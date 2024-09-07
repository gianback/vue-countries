<script lang="ts">
import { ref } from 'vue'

export default {
  setup() {
    const regions = ref(['Antarctic', 'Americas', 'Europe', 'Africa', 'Asia', 'Oceania'])
    return {
      regions
    }
  }
}
</script>

<template>
  <form>
    <select name="" id="">
      <option v-for="region in regions" :value="region" :key="region">
        {{ region }}
      </option>
    </select>
  </form>
</template>
