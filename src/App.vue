<script setup lang="ts">
import { RouterView } from 'vue-router'
import FooterApp from '@/components/FooterApp.vue'
import HeaderApp from '@/components/HeaderApp.vue'
</script>

<template>
  <HeaderApp />
  <RouterView />
  <FooterApp />
</template>
