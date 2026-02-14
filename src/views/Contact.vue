<template>
  <section id="contact" class="flex flex-col items-center justify-center bg-[#171616] py-16 md:py-20 overflow-hidden">
    <div class="container mx-auto px-4 sm:px-6 text-center">

      <!-- Header -->
      <div class="max-w-3xl mx-auto mb-10 md:mb-12">
        <h2 class="text-3xl sm:text-4xl md:text-5xl lg:text-7xl font-bold text-white mb-2 flex items-center justify-center gap-3 md:gap-4">
          <span class="text-cyan-400 font-mono text-base md:text-lg">06.</span>
          Contact
        </h2>
        <p class="text-slate-400 text-base sm:text-lg md:text-xl">ช่องทางการติดต่อ</p>
      </div>

      <!-- Contact Cards -->
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 sm:gap-6 md:gap-8 max-w-5xl mx-auto">
        <!-- Email -->
        <div
          class="bg-slate-800/20 border border-slate-700/50 rounded-2xl p-6 md:p-8 hover:border-cyan-400/50 hover:shadow-lg hover:shadow-cyan-500/20 transition-all duration-300">
          <h3 class="text-xl md:text-2xl font-bold text-white mb-3 md:mb-4">Email</h3>
          <p class="text-slate-400 mb-4 md:mb-6 break-all text-sm md:text-base">thanatchaya987@gmail.com</p>
          <a href="https://mail.google.com/mail/?view=cm&fs=1&to=thanatchaya987@gmail.com&su=&body=" target="_blank"
            rel="noopener noreferrer"
            class="inline-block w-full sm:w-auto px-5 md:px-6 py-2.5 md:py-3 rounded-lg bg-cyan-400 text-slate-950 font-semibold shadow-md hover:bg-cyan-500 hover:scale-105 active:scale-95 transition-all duration-300 cursor-pointer text-sm md:text-base">
            Send Email
          </a>
        </div>

        <!-- Phone -->
        <div
          class="bg-slate-800/20 border border-slate-700/50 rounded-2xl p-6 md:p-8 hover:border-cyan-400/50 hover:shadow-lg hover:shadow-cyan-500/20 transition-all duration-300">
          <h3 class="text-xl md:text-2xl font-bold text-white mb-3 md:mb-4">Phone</h3>
          <p class="text-slate-400 mb-4 md:mb-6 text-sm md:text-base">094-804-2979</p>
          <a href="tel:+66948042979"
            class="inline-block w-full sm:w-auto px-5 md:px-6 py-2.5 md:py-3 rounded-lg bg-cyan-400 text-slate-950 font-semibold shadow-md hover:bg-cyan-500 hover:scale-105 active:scale-95 transition-all duration-300 cursor-pointer text-sm md:text-base">
            Call Now
          </a>
        </div>

        <!-- Line -->
        <div
          class="bg-slate-800/20 border border-slate-700/50 rounded-2xl p-6 md:p-8 hover:border-cyan-400/50 hover:shadow-lg hover:shadow-cyan-500/20 transition-all duration-300 sm:col-span-2 md:col-span-1">
          <h3 class="text-xl md:text-2xl font-bold text-white mb-3 md:mb-4">Line</h3>
          <p class="text-slate-400 mb-4 md:mb-6 text-sm md:text-base">tnyb5</p>
          <a href="https://line.me/ti/p/tnyb5" target="_blank" rel="noopener noreferrer"
            class="inline-block w-full sm:w-auto px-5 md:px-6 py-2.5 md:py-3 rounded-lg bg-cyan-400 text-slate-950 font-semibold shadow-md hover:bg-cyan-500 hover:scale-105 active:scale-95 transition-all duration-300 cursor-pointer text-sm md:text-base">
            Add Line
          </a>
        </div>
      </div>

      <!-- Thank You Message -->
      <p class="text-slate-400 mt-12 md:mt-16 max-w-3xl mx-auto text-base sm:text-lg md:text-xl leading-relaxed px-4">
        ขอบคุณสำหรับโอกาสในการสมัครงานครั้งนี้
      </p>
      <p class="text-slate-400 mt-3 md:mt-4 max-w-3xl mx-auto text-base sm:text-lg md:text-xl leading-relaxed px-4">
        หวังเป็นอย่างยิ่งว่าจะได้ร่วมงานและเป้นส่วนหนึ่งขององค์กรที่พร้อมเติบโตไปด้วยกันในอนาคต
      </p>

    </div>
  </section>
</template>

<script setup lang="ts">
// ไม่มี props หรือ logic เพิ่มเติม
</script>

<style scoped>
@keyframes float {

  0%,
  100% {
    transform: translateY(0);
  }

  50% {
    transform: translateY(-5px);
  }
}

a:hover {
  animation: float 1s ease-in-out infinite alternate;
}
</style>