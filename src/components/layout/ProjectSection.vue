<script setup>
import ProjectCard from '../ui/ProjectCard.vue'
import project1 from '../../assets/project1.png'
import project2 from '../../assets/project2.png'
import project3 from '../../assets/project3.png'


const projects = [
  {
    icon: project1,
    title: 'HTML & CSS',
    description: 'Semantic, responsive, and modern layout using clean HTML structure and well-organized CSS styling techniques. Ensures accessibility and cross-device compatibility.',
  },
  {
    icon: project2,
    title: 'Vue.js',
    description: 'SPA and modular components using Vue. Features reactive data binding, component reusability, and clean structure for maintainable web apps.',
  },
  {
    icon: project3,
    title: 'Tailwind CSS',
    description: 'Utility-first CSS for fast and consistent design. Enables rapid UI building with low-level utility classes while maintaining design consistency.',
  }
]

</script>

<template>
    <section id="Project" class="relative py-25 px-4 sm:px-6 lg:px-8 max-w-6xl mx-auto min-h-screen">
        <div class="absolute w-1/2 aspect-[16/5] -skew-x-12 rounded-full 
      bg-gradient-to-r from-primary via-[#5C8374] to-secondary 
      opacity-20 dark:opacity-10 blur-[120px] left-10 top-0"></div>

        <div class="absolute w-1/2 aspect-[16/5] skew-x-12 rounded-full 
      bg-gradient-to-l from-primary via-[#5C8374] to-secondary 
      opacity-20 dark:opacity-10 blur-[120px] right-10 bottom-0"></div>

        <!-- Konten Utama -->
        <div class="relative z-10">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-secondary mb-12" data-aos="fade-down">
                Project
            </h2>

            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
                <ProjectCard v-for="(project, index) in projects" :key="index" :icon="project.icon"
                    :title="project.title" :description="project.description" data-aos="fade-right" />
            </div>
        </div>
    </section>
</template>
