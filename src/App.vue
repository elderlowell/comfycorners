<script setup lang="ts">
import { RouterView } from 'vue-router'
import HeaderBar from './components/HeaderBar.vue'
import FooterBar from './components/FooterBar.vue'
</script>

<template>
  <div class="relative min-h-dvh">
    <HeaderBar />
    <div class="pb-16">
      <RouterView />
    </div>
    <FooterBar />
  </div>
</template>
