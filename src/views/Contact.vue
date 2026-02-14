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
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 md:gap-8 max-w-5xl mx-auto mb-12">
        <!-- Email Card -->
        <div class="group bg-gradient-to-br from-slate-800/40 to-slate-900/40 backdrop-blur-sm border border-slate-700/50 rounded-2xl p-8 hover:border-cyan-400/60 hover:shadow-2xl hover:shadow-cyan-500/30 transition-all duration-500 hover:-translate-y-2">
          <div class="w-16 h-16 mx-auto mb-4 bg-gradient-to-br from-cyan-400 to-blue-500 rounded-xl flex items-center justify-center shadow-lg group-hover:scale-110 transition-transform duration-300">
            <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/>
            </svg>
          </div>
          <h3 class="text-2xl font-bold text-white mb-3">Email</h3>
          <p class="text-slate-300 mb-6 break-all text-sm">thanatchaya987@gmail.com</p>
          <a 
            href="mailto:thanatchaya987@gmail.com" 
            rel="noopener noreferrer"
            class="inline-block w-full px-6 py-3 rounded-xl bg-gradient-to-r from-cyan-400 to-blue-500 text-white font-semibold shadow-lg hover:shadow-cyan-500/50 hover:scale-105 active:scale-95 transition-all duration-300">
            ส่ง Email
          </a>
        </div>

        <!-- Phone Card -->
        <div class="group bg-gradient-to-br from-slate-800/40 to-slate-900/40 backdrop-blur-sm border border-slate-700/50 rounded-2xl p-8 hover:border-green-400/60 hover:shadow-2xl hover:shadow-green-500/30 transition-all duration-500 hover:-translate-y-2">
          <div class="w-16 h-16 mx-auto mb-4 bg-gradient-to-br from-green-400 to-emerald-500 rounded-xl flex items-center justify-center shadow-lg group-hover:scale-110 transition-transform duration-300">
            <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/>
            </svg>
          </div>
          <h3 class="text-2xl font-bold text-white mb-3">Phone</h3>
          <p class="text-slate-300 mb-6 text-lg font-mono">094-804-2979</p>
          <a 
            href="tel:+66948042979"
            class="inline-block w-full px-6 py-3 rounded-xl bg-gradient-to-r from-green-400 to-emerald-500 text-white font-semibold shadow-lg hover:shadow-green-500/50 hover:scale-105 active:scale-95 transition-all duration-300">
            โทรเลย
          </a>
        </div>

        <!-- Line Card -->
        <div class="group bg-gradient-to-br from-slate-800/40 to-slate-900/40 backdrop-blur-sm border border-slate-700/50 rounded-2xl p-8 hover:border-green-400/60 hover:shadow-2xl hover:shadow-green-500/30 transition-all duration-500 hover:-translate-y-2 sm:col-span-2 md:col-span-1">
          <div class="w-16 h-16 mx-auto mb-4 bg-gradient-to-br from-green-400 to-green-600 rounded-xl flex items-center justify-center shadow-lg group-hover:scale-110 transition-transform duration-300">
            <svg class="w-8 h-8 text-white" viewBox="0 0 24 24" fill="currentColor">
              <path d="M19.365 9.863c.349 0 .63.285.63.631 0 .345-.281.63-.63.63H17.61v1.125h1.755c.349 0 .63.283.63.63 0 .344-.281.629-.63.629h-2.386c-.345 0-.627-.285-.627-.629V8.108c0-.345.282-.63.63-.63h2.386c.346 0 .627.285.627.63 0 .349-.281.63-.63.63H17.61v1.125h1.755zm-3.855 3.016c0 .27-.174.51-.432.596-.064.021-.133.031-.199.031-.211 0-.391-.09-.51-.25l-2.443-3.317v2.94c0 .344-.279.629-.631.629-.346 0-.626-.285-.626-.629V8.108c0-.27.173-.51.43-.595.06-.023.136-.033.194-.033.195 0 .375.104.495.254l2.462 3.33V8.108c0-.345.282-.63.63-.63.345 0 .63.285.63.63v4.771zm-5.741 0c0 .344-.282.629-.631.629-.345 0-.627-.285-.627-.629V8.108c0-.345.282-.63.63-.63.346 0 .628.285.628.63v4.771zm-2.466.629H4.917c-.345 0-.63-.285-.63-.629V8.108c0-.345.285-.63.63-.63.348 0 .63.285.63.63v4.141h1.756c.348 0 .629.283.629.63 0 .344-.282.629-.629.629M24 10.314C24 4.943 18.615.572 12 .572S0 4.943 0 10.314c0 4.811 4.27 8.842 10.035 9.608.391.082.923.258 1.058.59.12.301.079.766.038 1.08l-.164 1.02c-.045.301-.24 1.186 1.049.645 1.291-.539 6.916-4.078 9.436-6.975C23.176 14.393 24 12.458 24 10.314"/>
            </svg>
          </div>
          <h3 class="text-2xl font-bold text-white mb-3">LINE</h3>
          <p class="text-slate-300 mb-4 text-lg font-mono">ID: tnyb5</p>
          
          <!-- วิธีเพิ่ม LINE ที่ถูกต้อง -->
          <div class="space-y-3">
            <!-- ปุ่มเปิดแอป LINE (แนะนำ) -->
            <a 
              href="https://line.me/ti/p/~tnyb5"
              target="_blank"
              rel="noopener noreferrer"
              class="inline-block w-full px-6 py-3 rounded-xl bg-gradient-to-r from-green-400 to-green-600 text-white font-semibold shadow-lg hover:shadow-green-500/50 hover:scale-105 active:scale-95 transition-all duration-300">
              เพิ่มเพื่อน LINE
            </a>
            
            <!-- QR Code (ถ้ามี) -->
            <div v-if="false" class="mt-4 p-4 bg-white rounded-xl">
              <img src="/src/assets/line.jfif" alt="LINE QR Code" class="w-32 h-32 mx-auto">
              <p class="text-slate-600 text-xs mt-2">สแกน QR Code</p>
            </div>
          </div>
        </div>
      </div>

      <!-- Thank You Message -->
      <p class="text-slate-400 mt-12 md:mt-16 max-w-3xl mx-auto text-base sm:text-lg md:text-xl leading-relaxed px-4">
        ขอบคุณสำหรับโอกาสในการสมัครงานครั้งนี้
      </p>
      <p class="text-slate-400 mt-3 md:mt-4 max-w-3xl mx-auto text-base sm:text-lg md:text-xl leading-relaxed px-4">
        หวังเป็นอย่างยิ่งว่าจะได้ร่วมงานและเป็นส่วนหนึ่งขององค์กรที่พร้อมเติบโตไปด้วยกันในอนาคต
      </p>

    </div>
  </section>
</template>

<script setup lang="ts">
// ไม่มี logic เพิ่มเติม
</script>

<style scoped>
a:hover {
  transform: scale(1.05);
  transition: transform 0.3s ease-in-out;
}
</style>
