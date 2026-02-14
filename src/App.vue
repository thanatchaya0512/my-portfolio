<template>
  <div class="font-inter">
    <Navbar />

    <!-- 1. Home Section -->
    <section id="home">
      <Home />
    </section>

    <!-- 2. About Section -->
    <section id="about">
      <About />
    </section>

    <!-- 3. Experience Section -->
    <section id="experience">
      <Experience />
    </section>

    <!-- 4. Skills Section -->
    <section id="skills">
      <Skill />
    </section>

    <!-- 5. Work Section -->
    <section id="work"> 
      <Work />
    </section>

    <!-- 6. Contact Section -->
    <section id="contact">
       <Contact />
    </section>
      
     
  </div>
</template>

<script setup lang="ts">
import Navbar from '@/components/Navbar.vue'
import Home from '@/views/Home.vue'
import About from '@/views/About.vue'
import Experience from '@/views/Experience.vue'
import Work from '@/views/Work.vue'
import Contact from '@/views/Contact.vue'
import Skill from '@/views/Skill.vue'
</script>

<style>
html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
</style>
