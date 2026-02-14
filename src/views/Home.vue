<template>
  <section id="home"
    class="relative min-h-screen flex items-center justify-center overflow-hidden
           bg-gradient-to-b from-[#171616] via-[#1f1e1e] to-[#171616]">

    <!-- Background grid -->
    <div class="absolute inset-0
             bg-[linear-gradient(to_right,#2a2a2a_1px,transparent_1px),
                 linear-gradient(to_bottom,#2a2a2a_1px,transparent_1px)]
             bg-[size:4rem_4rem]
             [mask-image:radial-gradient(ellipse_80%_50%_at_50%_50%,#000_70%,transparent_110%)]
             opacity-30" />

    <!-- Floating decorations -->
    <div class="absolute inset-0 pointer-events-none">
      <div class="absolute top-1/4 left-[10%] w-32 h-32 animate-float-slow opacity-30">
        <div
          class="w-full h-full rounded-xl bg-orange-600/20 border border-orange-500/30 backdrop-blur-sm rotate-12">
        </div>
      </div>

      <div class="absolute top-1/3 right-[15%] w-24 h-24 animate-float-medium opacity-40">
        <div
          class="w-full h-full rounded-xl bg-cyan-500/20 border border-cyan-400/30 backdrop-blur-sm -rotate-12">
        </div>
      </div>

      <div class="absolute bottom-[25%] left-[15%] w-40 h-40 blur-3xl bg-orange-600/20 rounded-full"></div>
      <div class="absolute top-[30%] right-[20%] w-40 h-40 blur-3xl bg-cyan-500/20 rounded-full"></div>
    </div>

    <!-- Content -->
    <div class="relative z-10 container mx-auto px-6">
      <div class="max-w-6xl mx-auto text-center">

        <!-- NAME -->
        <h1 class="text-5xl sm:text-7xl md:text-8xl lg:text-9xl
                 font-extrabold text-white tracking-tight leading-[0.95] mb-4">

          <span v-for="(char, i) in firstName" :key="i"
            class="inline-block opacity-0 animate-fade-in-up"
            :style="`animation-delay: ${0.1 + i * 0.05}s; animation-fill-mode: forwards;`">
            {{ char }}
          </span>

          <span class="block mt-2 text-3xl sm:text-4xl md:text-5xl
                   font-bold text-slate-300 tracking-wide">
            <span v-for="(char, i) in lastName" :key="'l' + i"
              class="inline-block opacity-0 animate-fade-in-up"
              :style="`animation-delay: ${0.7 + i * 0.05}s; animation-fill-mode: forwards;`">
              {{ char }}
            </span>
          </span>
        </h1>

        <h3
          class="text-xl sm:text-2xl text-slate-400 mt-4 opacity-0 animate-fade-in"
          style="animation-delay: 1s; animation-fill-mode: forwards;">
          ธนัชญา บิลายง๊ะ
        </h3>

        <!-- Divider -->
        <div class="mx-auto mt-6 h-px w-24
                 bg-gradient-to-r from-transparent via-cyan-400 to-transparent
                 opacity-0 animate-fade-in"
          style="animation-delay: 1.1s; animation-fill-mode: forwards;"></div>

        <!-- Subtitle -->
        <p class="mt-6 text-base sm:text-lg md:text-xl
                 text-slate-300 font-mono uppercase
                 tracking-[0.25em] opacity-0 animate-fade-in"
          style="animation-delay: 1.2s; animation-fill-mode: forwards;">
          Automation Engineer · Full Stack Developer
        </p>

        <!-- CTA -->
        <div class="mt-14 flex flex-col sm:flex-row gap-4 justify-center items-center
                 opacity-0 animate-fade-in"
          style="animation-delay: 1.4s; animation-fill-mode: forwards;">

          <a href="#work"
            @click.prevent="scrollToSection('work')"
            class="group px-8 py-4 rounded-xl
                   bg-gradient-to-r from-cyan-400 to-blue-500
                   text-[#171616] font-semibold
                   transition-all duration-300
                   hover:scale-105 hover:shadow-xl hover:shadow-cyan-500/30">
            View My Work
            <span class="inline-block ml-2 transition-transform group-hover:translate-x-1">→</span>
          </a>

          <a href="#contact"
            @click.prevent="scrollToSection('contact')"
            class="px-8 py-4 rounded-xl
                   border border-slate-600/60
                   text-slate-300
                   hover:text-white hover:border-cyan-400
                   hover:bg-[#1f1e1e]
                   transition-all duration-300">
            Get In Touch
          </a>
        </div>
      </div>
    </div>

    <!-- Scroll indicator -->
    <div class="absolute bottom-8 left-1/2 -translate-x-1/2 animate-bounce">
      <div class="w-6 h-10 border-2 border-slate-600 rounded-full flex justify-center pt-2">
        <div class="w-1 h-2 bg-cyan-400 rounded-full animate-pulse"></div>
      </div>
    </div>

  </section>
</template>

<script setup lang="ts">
const firstName = 'Thanatchaya'.split('')
const lastName = 'Bilainga'.split('')

const scrollToSection = (id: string) => {
  const el = document.getElementById(id)
  if (!el) return

  const offset = 80
  const top = el.getBoundingClientRect().top + window.pageYOffset - offset

  window.scrollTo({
    top,
    behavior: 'smooth'
  })
}
</script>

<style scoped>
@keyframes fade-in-up {
  from {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes fade-in {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}

@keyframes float-slow {

  0%,
  100% {
    transform: translateY(0) rotate(0deg);
  }

  50% {
    transform: translateY(-20px) rotate(6deg);
  }
}

@keyframes float-medium {

  0%,
  100% {
    transform: translateY(0) rotate(0deg);
  }

  50% {
    transform: translateY(-30px) rotate(-6deg);
  }
}

.animate-fade-in-up {
  animation: fade-in-up 0.6s ease-out;
}

.animate-fade-in {
  animation: fade-in 0.8s ease-out;
}

.animate-float-slow {
  animation: float-slow 6s ease-in-out infinite;
}

.animate-float-medium {
  animation: float-medium 4s ease-in-out infinite;
}
</style>
