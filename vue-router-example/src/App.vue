<script setup>
import { RouterLink, RouterView } from 'vue-router';

import AppHeader from '@/components/AppHeader.vue';
import AppContent from '@/components/AppContent.vue';
</script>

<template>
  <AppHeader></AppHeader>
  <AppContent></AppContent>
</template>

<style>
@import '@/assets/base.css';

body #app {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: 100%;
  min-height: 1rem;
}

body #app #app-header {
  flex: 0 0 auto;
}

body #app #app-content-container {
  flex: 1 1 auto;
}    
</style>
