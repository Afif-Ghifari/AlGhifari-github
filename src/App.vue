<template>
  <header>
    <HeaderComponent />
  </header>
  <main>
    <HeroComponent />
    <About id="about" />
    <Experience id="experience" />
  </main>
</template>

<script setup>
import HeaderComponent from './components/Header.vue';
import HeroComponent from './components/Hero.vue'
import About from './components/About.vue';
import Experience from './components/Experience.vue';
</script>

<style scoped>
</style>
