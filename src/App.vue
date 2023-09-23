<template>
  <header>
    <HeaderComponent />
  </header>
  <main>
    <HeroComponent />
    <About />
  </main>
</template>

<script setup>
import HeaderComponent from './components/Header.vue';
import HeroComponent from './components/Hero.vue'
import About from './components/About.vue';
</script>

<style scoped>
</style>
