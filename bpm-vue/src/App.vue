<script setup>
import { RouterView } from 'vue-router'
import FooterBar from './components/FooterBar.vue';
import NavBar from './components/NavBar.vue';
</script>

<template>
  <NavBar />
  <RouterView />
  <FooterBar />
</template>

<style scoped></style>
