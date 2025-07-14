<script setup>
import SkillIcon from '../ui/SkillIcon.vue'
import html from '../../assets/icon/html.svg'
import css from '../../assets/icon/css.svg'
import js from '../../assets/icon/javascript.svg'
import vue from '../../assets/icon/vue.svg'
import react from '../../assets/icon/react.svg'

const skills = [
    { icon: html, label: 'HTML' },
    { icon: css, label: 'CSS' },
    { icon: js, label: 'JavaScript' },
    { icon: vue, label: 'Vue.js' },
    { icon: react, label: 'React' }
]
</script>

<template>
  <section id="Skill" class="relative py-25 px-4 max-w-6xl mx-auto min-h-screen">
    <div class="absolute w-1/2 aspect-[16/5] -skew-x-12 rounded-full 
      bg-gradient-to-r from-[#183D3D] via-[#5C8374] to-secondary 
      opacity-30 blur-[100px] left-10 top-0 block"></div>

    <div class="absolute w-1/2 aspect-[16/5] skew-x-12 rounded-full 
      bg-gradient-to-l from-[#183D3D] via-[#5C8374] to-secondary 
      opacity-30 blur-[100px] right-10 bottom-0 block"></div>

    <div class="relative z-10">
      <h2 class="text-3xl md:text-4xl font-bold text-center text-secondary mb-10" data-aos="fade-down">
        My Skill
      </h2>

      <!-- Added description -->
      <p class="text-center text-white max-w-xl mx-auto mb-6" data-aos="fade-up">
        These are the technologies I specialize in and frequently use to build modern web applications.
      </p>

      <div class="grid grid-cols-3 sm:grid-cols-4 md:grid-cols-5 gap-6 place-items-center">
        <SkillIcon 
          v-for="(skill, index) in skills" 
          :key="index" 
          :icon="skill.icon" 
          :label="skill.label" 
          class="mt-10" 
          data-aos="fade-right" 
        />
      </div>
    </div>
  </section>
</template>


