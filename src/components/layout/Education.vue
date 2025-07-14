<template>
  <section id="Education" class="relative py-25 px-4 sm:px-6 lg:px-8 max-w-6xl mx-auto min-h-screen">
    <!-- Background blur kiri -->
    <div
      class="absolute w-1/2 aspect-[16/5] -skew-x-12 rounded-full 
      bg-gradient-to-r from-primary via-[#5C8374] to-secondary 
      opacity-20 dark:opacity-10 blur-[120px] left-10 top-0">
    </div>

    <!-- Background blur kanan -->
    <div
      class="absolute w-1/2 aspect-[16/5] skew-x-12 rounded-full 
      bg-gradient-to-l from-primary via-[#5C8374] to-secondary 
      opacity-20 dark:opacity-10 blur-[120px] right-10 bottom-0">
    </div>

    <!-- Konten utama -->
    <div class="relative z-10">
      <h2 class="text-3xl md:text-4xl font-bold text-center text-secondary mb-12" data-aos="fade-down">
        Education
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
        <!-- Text pendidikan -->
        <div class="space-y-6 text-white/80" data-aos="fade-right">
          <div>
            <h3 class="text-xl font-semibold text-white">Informatics Engineering</h3>
            <p class="text-sm text-white/60">Universitas Islam Riau • 2023 - Now</p>
            <p class="mt-2">
              Studied software development, data structures, networks, and algorithm optimization. Focused on building reliable and efficient systems.
            </p>
          </div>
        </div>

        <!-- Gambar atau ilustrasi -->
        <figure class="w-full max-w-sm mx-auto rounded-xl overflow-hidden shadow-lg" data-aos="fade-left">
          <img :src="educationImg" alt="Education" class="w-full h-full object-cover" />
        </figure>
      </div>
    </div>
  </section>
</template>

<script setup>
import educationImg from '../../assets/education.jpg'
</script>
