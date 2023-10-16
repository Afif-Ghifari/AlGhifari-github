<template>
  <header>
    <HeaderComponent />
  </header>
//main content 
  <main>
    <HeroComponent />
    <About id="about" />
    <Experience id="experience" />
    <Education id="education" />
    <Projects id="projects" />
    <Skill id="skill"/>
    <Contact id="contact"/>
    <FooterVue />
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
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';
import FooterVue from './components/Footer.vue';
</script>

<style scoped>
</style>
