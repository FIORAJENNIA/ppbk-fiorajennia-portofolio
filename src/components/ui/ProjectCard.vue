<script setup>
defineProps({
  icon: String,
  title: String,
  description: String,
  codeLink: {
    type: String,
    default: 'test',
  },
})
</script>

<template>
  <div
    class="bg-white/10 backdrop-blur-lg p-6 rounded-2xl shadow-md hover:shadow-xl transition-all duration-300 text-center flex flex-col justify-between h-full border border-white/10 hover:border-secondary/50">
    <div>
      <img :src="icon" alt="Project Icon"
        class="w-auto h-52 mx-auto mb-5 rounded-2xl border-4 border-primary shadow-sm object-cover" />
      <h3 class="text-xl font-semibold text-secondary mb-2 tracking-wide">{{ title }}</h3>
      <p class="text-sm text-white/80 leading-relaxed text-justify">{{ description }}</p>
    </div>


  </div>
</template>
