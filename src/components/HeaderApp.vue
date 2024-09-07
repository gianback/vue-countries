<script lang="ts">
import { ref } from 'vue'

export default {
  setup() {
    const theme = ref(false)

    function handleTheme() {
      theme.value = !theme.value
    }

    return {
      theme,
      handleTheme
    }
  }
}
</script>

<template>
  <header class="bg-bg-light p-8 shadow-md">
    <div class="flex items-center justify-between">
      <nav class="flex gap-4 items-center">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/favorites">My Favorites Countries</RouterLink>
      </nav>
      <button @click="handleTheme">{{ theme ? 'Dark' : 'Light' }} Mode</button>
    </div>
  </header>
</template>
