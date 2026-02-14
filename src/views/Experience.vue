<template>
  <section id="experience" class="flex items-center justify-center bg-[#171616] py-20 overflow-hidden">
    <div class="container mx-auto px-6 relative z-10">

      <!-- Section Header -->
      <div class="max-w-6xl mx-auto mb-20">
        <h2 class="text-4xl md:text-5xl font-bold text-white mb-2 flex items-center group">
          <span class="text-cyan-400 font-mono text-xl mr-4 opacity-80">03.</span>
          <span class="group-hover:text-cyan-400 transition-colors duration-300">EXPERIENCE</span>
          <div class="hidden md:block h-[1px] flex-1 max-w-xs bg-slate-700 ml-8"></div>
        </h2>
        <p class="text-slate-300 font-mono text-ls uppercase tracking-[0.2em] ml-12">ประสบการณ์การทำงาน</p>
      </div>

      <!-- Timeline -->
      <div class="max-w-5xl mx-auto relative">
        <!-- Vertical Line - ซ่อนบนมือถือ -->
        <div class="hidden md:block absolute left-0 md:left-1/2 md:-translate-x-1/2 top-0 bottom-0 w-[2px] bg-slate-800/50">
          <div
            class="absolute top-0 left-0 w-full bg-gradient-to-b from-cyan-500 to-blue-500 shadow-[0_0_10px_rgba(6,182,212,0.5)] transition-all duration-200"
            :style="{ height: scrollPercent + '%' }">
            <div
              class="absolute bottom-0 left-1/2 -translate-x-1/2 w-3 h-3 bg-white rounded-full border-2 border-cyan-400 shadow-[0_0_15px_#22d3ee]">
            </div>
          </div>
        </div>

        <!-- Timeline Items -->
        <div class="space-y-12 md:space-y-28">

          <!-- Job 1 -->
          <div class="relative grid md:grid-cols-2 gap-6 md:gap-12 items-start">
            <div class="md:text-left">
              <span class="text-cyan-400 font-mono font-medium text-sm md:text-base">6 พฤษภาคม 2568 — ปัจจุบัน</span>
              <h3 class="text-xl md:text-2xl font-bold text-white mt-2">Automation Engineer (Programmer)</h3>
              <p class="text-slate-400 text-base md:text-lg">บริษัท พรีเมียร์ซิสเต็มเอ็นจิเนียริ่ง จำกัด</p>
            </div>
            <div
              class="bg-slate-800/30 p-6 md:p-8 rounded-2xl border border-white/5 hover:border-cyan-400/30 transition-all group shadow-lg hover:shadow-cyan-500/30">
              <ul class="space-y-3 md:space-y-4 text-slate-300 text-sm md:text-base">
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ออกแบบและพัฒนา เว็บแดชบอร์ด แสดงข้อมูลเรียลไทม์จากระบบหลังบ้าน รองรับการพัฒนาต่อโดยทีม</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>เขียนโค้ดเพื่อจัดการข้อมูลหลังบ้านและส่งต่อให้หน้าเว็บแสดงผลอย่างมีประสิทธิภาพ</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ใช้ Axios และ Socket.io ในการสื่อสารข้อมูลระหว่าง Frontend และ Backend</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>พัฒนาระบบ Forward Notification สำหรับเก็บ Log และให้แอดมินเพิ่ม/ลบ/แก้ไขรายการได้ พร้อมระบบ JWT
                    และ Token เชื่อมต่อฐานข้อมูล SQL, Docker, และ Git สำหรับการ Deploy และแก้ไขปัญหาในการ Deploy
                    ร่วมกับทีมพัฒนา</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ตั้งค่าและพัฒนา ระบบตรวจจับการเคลื่อนไหวของผลิตภัณฑ์ ด้วยกล้อง โดยใช้ Python
                    เพื่อส่งต่อข้อมูลให้ทีมพัฒนาต่อ</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ออกแบบ โครงสร้างเว็บและ UI ผ่าน Figma ร่วมกับทีม</span>
                </li>
              </ul>
              <div class="mt-6 md:mt-8 flex flex-wrap gap-2">
                <span
                  v-for="t in ['TS', 'JS', 'Python', 'HTML', 'CSS', 'Bootstrap', 'Vue', 'NodeJs', 'SQL', 'Management', 'Docker', 'Socket.io', 'API', 'FastAPI', 'OpenCV', 'GitLab']"
                  :key="t"
                  class="px-2 py-1 bg-cyan-400/10 text-cyan-400 text-[10px] rounded font-mono border border-cyan-400/20">{{
                  t }}</span>
              </div>
            </div>
          </div>

          <!-- Job 2 -->
          <div class="relative flex flex-col md:flex-row md:items-start gap-6 md:gap-12">
            <!-- Left / Right Info -->
            <div class="md:w-1/2 md:text-left">
              <span class="text-cyan-400 font-mono font-medium text-sm md:text-base">18 พฤศจิกายน 2567 — 8 มีนาคม 2568</span>
              <h3 class="text-xl md:text-2xl font-bold text-white mt-2">Programmer (นักศึกษาฝึกงาน)</h3>
              <p class="text-slate-400 text-base md:text-lg">มหาวิทยาลัยหาดใหญ่</p>
            </div>

            <!-- Card -->
            <div
              class="md:w-1/2 bg-slate-800/30 p-6 md:p-8 rounded-2xl border border-white/5 shadow-lg hover:shadow-cyan-500/20 transition-all hover:border-cyan-400/30">
              <ul class="space-y-3 text-slate-300 text-sm md:text-base">
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ออกแบบหน้าเว็บไซต์ลงทะเบียนเข้าร่วมงานมหาวิทยาลัย</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ออกแบบฐานข้อมูลเพื่อใช้ในการสร้างระบบล็อคอินและจัดการเซสชั่นของผู้ใช้</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>พัฒนาระบบล็อคอินที่เชื่อมต่อกับ Facebook เพื่อให้ผู้ใช้สามารถล็อกอินได้สะดวก</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ทำการวิเคราะห์ข้อมูลใน Excel และนำข้อมูลไปแสดงผลบน Looker Studio
                    เพื่อการรายงานและวิเคราะห์ที่ชัดเจน</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ปรับปรุงการออกแบบเว็บไซต์ให้ตรงกับความต้องการของผู้ใช้</span>
                </li>
              </ul>

              <!-- Skill Tags -->
              <div class="mt-6 flex flex-wrap gap-2 md:justify-end">
                <span v-for="t in ['PHP', 'SQL', 'Xampp', 'HTML', 'CSS']" :key="t"
                  class="px-3 py-1 bg-slate-700/30 text-slate-400 text-xs rounded font-mono border border-slate-700">{{
                  t }}</span>
              </div>
            </div>
          </div>

          <!-- Job 3 -->
          <div class="relative grid md:grid-cols-2 gap-6 md:gap-12 items-start">
            <div class="md:w-1/1 md:text-left">
              <span class="text-cyan-400 font-mono font-medium text-sm md:text-base">1 เมษายน 2567 — 31 พฤษภาคม 2567</span>
              <h3 class="text-xl md:text-2xl font-bold text-white mt-2">Technical Support (นักศึกษาฝึกงาน)</h3>
              <p class="text-slate-400 text-base md:text-lg">บริษัท เอ็กซ์เพรส ดาต้า จำกัด</p>
            </div>
            <div
              class="bg-slate-800/30 p-6 md:p-8 rounded-2xl border border-white/5 hover:border-slate-400/30 transition-all shadow-lg hover:shadow-slate-400/20">
              <ul class="space-y-3 md:space-y-4 text-slate-300 text-sm md:text-base">
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ศึกษาและเรียนรู้เกี่ยวกับระบบเน็ตเวิร์กและเครือข่ายคอมพิวเตอร์ รวมถึงการคำนวณ IP Address</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ศึกษาเรียนรู้การคอนฟิกเราท์เตอร์และสวิตช์โดยใช้ Cisco</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>เก็บบันทึก Log ของระบบกล้องวงจรปิดของลูกค้า ทั้งรีโมตและออนไซต์</span>
                </li>
                <li class="flex gap-2 items-start">
                  <span class="text-cyan-400 mt-1">▸</span>
                  <span>ทำการบริการหลังการขายและ PM (Preventive Maintenance) นอกสถานที่</span>
                </li>
              </ul>
              <div class="mt-6 md:mt-8 flex flex-wrap gap-2">
                <span
                  class="px-2 py-1 bg-slate-700/30 text-slate-400 text-[10px] rounded font-mono border border-slate-700 uppercase">Cisco</span>
                <span
                  class="px-2 py-1 bg-slate-700/30 text-slate-400 text-[10px] rounded font-mono border border-slate-700 uppercase">PM
                  Services</span>
              </div>
            </div>
          </div>

        </div>
      </div>

    </div>
  </section>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue';

const scrollPercent = ref(0);

const handleScroll = () => {
  const section = document.getElementById('experience');
  if (!section) return;

  const rect = section.getBoundingClientRect();
  const windowHeight = window.innerHeight;
  const sectionHeight = section.offsetHeight;

  const start = rect.top - windowHeight / 2;
  const current = -start;
  const rawPercent = (current / sectionHeight) * 100;
  scrollPercent.value = Math.min(Math.max(rawPercent, 0), 100);
};

onMounted(() => window.addEventListener('scroll', handleScroll));
onUnmounted(() => window.removeEventListener('scroll', handleScroll));
</script>