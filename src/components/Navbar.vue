<script setup lang="ts">
import { ref } from 'vue';
const mobileMenuOpen = ref(false);
const navItems = [
  { id: 'home', label: 'home', number: '01' },
  { id: 'about', label: 'about', number: '02' },
  { id: 'experience', label: 'experience', number: '03' },
  { id: 'skills', label: 'skills', number: '04' },
  { id: 'work', label: 'projects', number: '05' },
  { id: 'contact', label: 'contact', number: '06' },
]

const scrollToSection = (id: string) => {
  const section = document.getElementById(id);
  if (section) {
    const offset = 80 ; // Adjust this value based on your navbar height
    const elementPosition = section.getBoundingClientRect().top
    const offsetPosition = elementPosition + window.pageYOffset - offset;
    window.scrollTo({
      top: offsetPosition,
      behavior: 'smooth'
    });

  }
};

const handleMobileClick = (sectionId: string) => {
  mobileMenuOpen.value = false
  scrollToSection(sectionId)
}
</script>
<template>
  <header
    class="fixed top-0 left-0 right-0 z-50 bg-slate-950/80 backdrop-blur-md border-b border-slate-800/50"
  >
    <div class="container mx-auto px-6 py-4">
      <nav class="flex items-center justify-between">
        <!-- Logo -->
        <a
          href="#home"
          class="text-cyan-400 text-xl font-bold font-mono hover:text-cyan-300 transition-colors"
        >
          DevM.<span class="animate-pulse">_</span>
        </a>
        <!-- Navigation Links -->
         <ul class="hidden md:flex item-center gap-8">
            <li v-for="item in navItems" :key="item.id">
                <a :href="`#${item.id}`" @click="scrollToSection(item.id)" class="group relative text-slate-300 hover:text-white transition-colors font-mono text-sm">{{ item.label }}
                   <span class="text-cyan-400 mr-1">{{ item.number }}</span>
              <span class="absolute -bottom-1 left-0 w-0 h-0.5 bg-cyan-400 group-hover:w-full transition-all duration-300"></span>
                </a>
            </li>   
         </ul>
       <!-- Mobile Menu Button -->
        <button 
          @click="mobileMenuOpen = !mobileMenuOpen"
          class="md:hidden text-slate-300 hover:text-white"
        >
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path v-if="!mobileMenuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </nav>

      <!-- Mobile Navigation -->
      <transition
        enter-active-class="transition duration-200 ease-out"
        enter-from-class="opacity-0 -translate-y-4"
        enter-to-class="opacity-100 translate-y-0"
        leave-active-class="transition duration-150 ease-in"
        leave-from-class="opacity-100 translate-y-0"
        leave-to-class="opacity-0 -translate-y-4"
      >
        <ul v-if="mobileMenuOpen" class="md:hidden mt-4 space-y-3 pb-4">
          <li v-for="item in navItems" :key="item.id">
            <a 
              :href="`#${item.id}`"
              @click="handleMobileClick(item.id)"
              class="block text-slate-300 hover:text-white hover:bg-slate-800/50 px-4 py-2 rounded transition-colors font-mono text-sm"
            >
              <span class="text-cyan-400 mr-2">{{ item.number }}</span>
              {{ item.label }}
            </a>
          </li>
        </ul>
      </transition>
    </div>
  </header>
</template>