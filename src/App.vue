<script setup>
import Header from './components/layout/Header.vue'
import HeroSection from './components/layout/HeroSection.vue'
import SkillSection from './components/layout/SkillSection.vue'
import ProjectSection from './components/layout/ProjectSection.vue'
import Contact from './components/layout/Contact.vue'
import Education from './components/layout/Education.vue'
</script>

<template>
  <div class="bg-primary font-display">
    <Header />
    <HeroSection />
    <SkillSection />
    <Education />
    <ProjectSection />
    <Contact />
  </div>
</template>

<style scoped></style>
