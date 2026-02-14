<template>
  <section id="work" class="bg-[#171616] py-24 relative overflow-hidden">

    <!-- Background Glow -->
    <div class="absolute top-1/4 -left-20 w-80 h-80 bg-cyan-500/5 rounded-full blur-[100px]"></div>
    <div class="absolute bottom-1/4 -right-20 w-80 h-80 bg-blue-500/5 rounded-full blur-[100px]"></div>

    <div class="container mx-auto px-6 relative z-10">

      <!-- Section Header -->
      <div class="max-w-6xl mx-auto mb-20">
        <h2 class="flex items-center text-3xl md:text-5xl font-bold text-white mb-4">
          <span class="text-cyan-400 font-mono text-lg mr-4">05.</span>
          <span class="hover:text-cyan-400 transition-colors">
            PROJECTS
          </span>
          <div class="hidden md:block h-[1px] flex-1 max-w-xs bg-slate-700 ml-8"></div>
        </h2>
        <p class="text-slate-400 font-mono text-xs md:text-sm uppercase tracking-[0.3em] ml-12">
          ผลงานและประสบการณ์ที่ผ่านมา
        </p>
      </div>

      <div class="max-w-6xl mx-auto space-y-28">

        <!-- ===== Project 1 - Forward Notification ===== -->
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 items-center fade-in">

          <!-- Image -->
          <div class="lg:col-span-7 relative">
            <div class="overflow-hidden rounded-xl border border-slate-700/40 shadow-2xl group">
              <div class="absolute inset-0 bg-cyan-900/20 group-hover:bg-transparent transition duration-500"></div>
              <img
                :src="forwardImages[0]"
                alt="Forward Notification"
                class="w-full object-cover transition duration-700 group-hover:scale-105"
              />
            </div>

            <!-- Floating Image -->
            <div class="hidden md:block absolute -bottom-6 -right-6 w-48 border-4 border-[#171616] rounded-lg shadow-xl overflow-hidden">
              <img src="/src/assets/log-noti.jfif" class="w-full object-cover" />
            </div>
          </div>

          <!-- Content -->
          <div class="lg:col-span-5 lg:text-right">

            <h3 class="text-xl md:text-3xl font-bold text-white mb-4 hover:text-cyan-400 transition">
              Forward Notification System
            </h3>

            <div class="bg-slate-900/60 backdrop-blur-xl border border-slate-700/40 p-6 rounded-lg shadow-xl mb-4">
              <p class="text-slate-300 text-sm md:text-base leading-relaxed">
                พัฒนาระบบแจ้งเตือนสถานะเครื่องจักร พร้อมระบบแอดมินที่ใช้ JWT
                เพื่อความปลอดภัย เชื่อมต่อฐานข้อมูล แสดงผล Log แบบ Real-time
                ทดสอบด้วย Postman แจ้งเตือนผ่าน MS Teams และ Deploy ผ่าน Docker ร่วมกับทีม
              </p>
            </div>

            <ul class="flex flex-wrap gap-3 lg:justify-end text-slate-400 font-mono text-xs">
              <li>Vue.js</li>
              <li>Node.js</li>
              <li>JWT</li>
              <li>Docker</li>
              <li>GitLab</li>
              <li>TypeScript</li>
              <li>Axios</li>
            </ul>
          </div>
        </div>

        <!-- ===== Project 2 - FeedControl Dashboard ===== -->
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 items-center fade-in">

          <!-- Image -->
          <div class="lg:col-span-7 relative">
            <div class="overflow-hidden rounded-xl border border-slate-700/40 shadow-2xl group">
              <div class="absolute inset-0 bg-cyan-900/20 group-hover:bg-transparent transition duration-500"></div>
              <img
                src="/src/assets/feedcontrol.jfif"
                alt="FeedControl Dashboard"
                class="w-full object-cover transition duration-700 group-hover:scale-105"
              />
            </div>
          </div>

          <!-- Content -->
          <div class="lg:col-span-5 lg:text-right">

            <h3 class="text-xl md:text-3xl font-bold text-white mb-4 hover:text-cyan-400 transition">
              FeedControl Dashboard
            </h3>

            <div class="bg-slate-900/60 backdrop-blur-xl border border-slate-700/40 p-6 rounded-lg shadow-xl mb-4">
              <p class="text-slate-300 text-sm md:text-base leading-relaxed">
                สร้าง Dashboard วิเคราะห์ข้อมูลเครื่องจักรด้วย TypeScript
                แสดงผลกราฟผ่าน ApexCharts และ Ant Design Vue
                เชื่อมต่อ API และรองรับข้อมูลแบบ Real-time
              </p>
            </div>

            <ul class="flex flex-wrap gap-3 lg:justify-end text-slate-400 font-mono text-xs">
              <li>Vue.js</li>
              <li>TypeScript</li>
              <li>Ant Design</li>
              <li>ApexCharts</li>
              <li>Socket.io</li>
            </ul>
          </div>
        </div>

        <!-- ===== Project 3 - Config Camera ===== -->
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 items-center fade-in">

          <!-- Camera Icon Design -->
          <div class="lg:col-span-7">
            <div class="aspect-video rounded-xl border border-slate-700/40 bg-gradient-to-br from-slate-900 via-slate-800 to-slate-900 flex items-center justify-center relative overflow-hidden group">
              <!-- Background Pattern -->
              <div class="absolute inset-0 opacity-5">
                <div class="absolute inset-0 bg-[linear-gradient(to_right,#4f4f4f_1px,transparent_1px),linear-gradient(to_bottom,#4f4f4f_1px,transparent_1px)] bg-[size:2rem_2rem]"></div>
              </div>
              
              <!-- Glow Effect -->
              <div class="absolute inset-0 bg-gradient-to-br from-cyan-500/10 via-transparent to-blue-500/10"></div>
              
              <!-- Camera Icon -->
              <div class="relative z-10 flex flex-col items-center gap-6">
                <svg xmlns="http://www.w3.org/2000/svg" class="w-32 h-32 text-cyan-400/80 group-hover:text-cyan-400 transition-all duration-500 group-hover:scale-110" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M3 9a2 2 0 012-2h.93a2 2 0 001.664-.89l.812-1.22A2 2 0 0110.07 4h3.86a2 2 0 011.664.89l.812 1.22A2 2 0 0018.07 7H19a2 2 0 012 2v9a2 2 0 01-2 2H5a2 2 0 01-2-2V9z" />
                  <path stroke-linecap="round" stroke-linejoin="round" d="M15 13a3 3 0 11-6 0 3 3 0 016 0z" />
                </svg>
                
                <div class="text-center">
                  <p class="text-slate-400 font-mono text-sm mb-1">OpenCV Vision System</p>
                  <p class="text-slate-600 font-mono text-xs">Motion Detection & Processing</p>
                </div>
              </div>
            </div>
          </div>

          <!-- Content -->
          <div class="lg:col-span-5 lg:text-right">

            <h3 class="text-xl md:text-3xl font-bold text-white mb-4 hover:text-cyan-400 transition">
              Config Camera
            </h3>

            <div class="bg-slate-900/60 backdrop-blur-xl border border-slate-700/40 p-6 rounded-lg shadow-xl mb-4">
              <p class="text-slate-300 text-sm md:text-base leading-relaxed">
                Config กล้องสำหรับตรวจจับการเคลื่อนไหวในกระบวนการผลิต
                ใช้ Python และ OpenCV ประมวลผลภาพ
                ตรวจจับจังหวะอัตโนมัติและส่งข้อมูลต่อทีมพัฒนา
              </p>
            </div>

            <ul class="flex flex-wrap gap-3 lg:justify-end text-slate-400 font-mono text-xs">
              <li>Python</li>
              <li>OpenCV</li>
              <li>Image Processing</li>
            </ul>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>

<script setup>
const forwardImages = [
  '/src/assets/modal-noti.jfif'
]
</script>

<style scoped>
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(40px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.fade-in {
  animation: fadeInUp 0.8s ease-out both;
}
</style>