<script setup lang="ts">
import { ref } from 'vue'

const search = ref('')
</script>

<template>
  <form action="">
    <input type="text" v-model.trim="search" />
  </form>
</template>
