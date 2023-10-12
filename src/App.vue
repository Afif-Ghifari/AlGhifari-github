<template>
  <header>
    <HeaderComponent />
  </header>
  <main>
    <HeroComponent />
    <About id="about" />
    <Experience id="experience" />
    <Education id="education" />
    <Projects id="projects" />
    <Skill id="skill"/>
  </main>
</template>

<script setup>
import 'bootstrap-icons/font/bootstrap-icons.css'
import HeaderComponent from './components/Header.vue';
import HeroComponent from './components/Hero.vue'
import About from './components/About.vue';
import Experience from './components/Experience.vue'
import Education from './components/Education.vue';
import Projects from './components/Projects.vue';
import Skill from './components/Skill.vue';
</script>

<style scoped>
</style>
