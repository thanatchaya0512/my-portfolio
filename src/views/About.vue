<template>
  <section id="about" class="min-h-screen flex items-center justify-center bg-[#171616] py-20 overflow-hidden">
    <div class="container mx-auto px-6 relative">
      <div class="absolute top-0 left-1/4 w-96 h-96 bg-cyan-500/5 rounded-full blur-[120px] -z-10 animate-pulse-slow"></div>
      <div class="absolute bottom-0 right-1/4 w-80 h-80 bg-blue-500/5 rounded-full blur-[100px] -z-10 animate-pulse-slow" style="animation-delay: 2s;"></div>
      
      <div class="max-w-6xl mx-auto">
        <div class="mb-12">
          <h2 class="text-4xl md:text-5xl font-bold text-white mb-2 flex items-center group">
            <span class="text-cyan-400 font-mono text-lg mr-4 opacity-80">02.</span>
            <span class="group-hover:text-cyan-400 transition-colors duration-300">About Me</span>
            <div class="hidden md:block h-[1px] flex-1 max-w-xs bg-slate-700 ml-8"></div>
          </h2>
          <p class="text-slate-300 font-mono text-ls uppercase tracking-[0.2em] ml-12">ข้อมูลส่วนตัว</p>
        </div>

        <div class="grid md:grid-cols-12 gap-12 items-start">
          
          <div class="md:col-span-4 space-y-8">
            <div class="relative group max-w-[280px] mx-auto md:mx-0">
              <div class="relative rounded-xl border border-cyan-400/20 p-2 transition-all duration-500 group-hover:-translate-y-2 group-hover:border-cyan-400/50">
                <div class="relative overflow-hidden rounded-lg bg-slate-800 aspect-[4/5]">
                 <img src="/src/assets/myphoto.png" alt="Thanatchaya Bilaynga" class="w-full h-full object-cover transition-all duration-700">

                  <div class="absolute inset-0 bg-cyan-900/10 group-hover:bg-transparent transition-all duration-500"></div>
                </div>
              </div>
              <div class="absolute inset-0 border-2 border-cyan-400/30 rounded-xl -z-10 translate-y-4 translate-x-4 group-hover:translate-y-2 group-hover:translate-x-2 transition-transform duration-500"></div>
              
              <div class="absolute -top-3 -right-3 bg-yellow-300 text-slate-900 font-bold px-3 py-1 rounded-md shadow-lg text-[12px] tracking-tighter animate-float">
                เกียรตินิยมอันดับ 2
              </div>
            </div>

            <div class="bg-slate-800/20 border border-slate-700/50 rounded-xl p-5 hover:border-cyan-400/30 transition-all duration-300 group">
              <h4 class="text-slate-200 font-semibold text-sm mb-4 flex items-center gap-2">
                <svg class="w-4 h-4 text-cyan-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path d="M12 14l9-5-9-5-9 5 9 5z"/><path d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"/>
                </svg>
                Education
              </h4>
              <div class="border-l-2 border-cyan-400/20 pl-4 py-1">
                <p class="text-xs font-mono text-cyan-400">2564 — 2568</p>
                <p class="text-white text-sm font-bold leading-tight mt-1">มหาวิทยาลัยสงขลานครินทร์</p>
                <p class="text-slate-400 text-xs mt-1">คณะบริหารธุรกิจ</p>
                <p class="text-slate-400 text-xs mt-1">สาขาระบบสารสนเทศทางธุรกิจ</p>
                <div class="mt-3 flex items-center gap-2">
                  <span class="text-[10px] bg-cyan-400/10 text-cyan-400 px-2 py-0.5 rounded border border-cyan-400/20 font-mono">GPA 3.56</span>
                </div>
              </div>
            </div>
          </div>

          <div class="md:col-span-8 space-y-10">
            
            <div class="space-y-4">
              <h3 class="text-3xl md:text-5xl font-bold text-white leading-tight">
                ธนัชญา บิลายง๊ะ <br/>
                <span class="text-xl md:text-2xl text-cyan-400/80 font-medium">Automation Engineer (Programmer)</span>
              </h3>
              <p class="text-slate-400 max-w-2xl leading-relaxed">
                กำลังมองหาโอกาสในการย้ายงานและพัฒนาทักษะในสายงาน <span class="text-slate-200">Full-stack Developer</span> เพื่อสร้างความเชี่ยวชาญครบวงจรทั้งด้าน Frontend และ Backend พร้อมเรียนรู้เทคโนโลยีใหม่ ๆ และสามารถออกแบบระบบที่สอดคล้องกับความต้องการทางธุรกิจ
              </p>
            </div>

            <div class="grid gap-8">
              <div class="relative pl-6">
                <div class="absolute left-0 top-0 bottom-0 w-[2px] bg-gradient-to-b from-cyan-400/50 to-transparent"></div>
                <h4 class="text-white font-bold mb-3 text-lg">เกี่ยวกับฉัน</h4>
                <p class="text-slate-400 leading-relaxed text-base">
                  ปัจจุบันรับหน้าที่เป็น <span class="text-white font-medium">Automation Engineer</span> ณ บริษัท พรีเมียร์ซิสเต็มเอ็นจิเนียริ่ง จำกัด โดยดูแลรับผิดชอบการพัฒนา <span class="text-cyan-400">Frontend-Backend</span> 
                  เพื่อรับข้อมูลจากเครื่องจักรอัตโนมัติมาประมวลผลและนำเสนอผ่าน <span class="text-white border-b border-cyan-400/30">Real-time Dashboards</span> 
                  ช่วยให้การวิเคราะห์ข้อมูลมีความแม่นยำและเข้าถึงง่ายขึ้น
                </p>
              </div>

              <div class="relative pl-6">
                <div class="absolute left-0 top-0 bottom-0 w-[2px] bg-gradient-to-b from-cyan-400/50 to-transparent"></div>
                <h4 class="text-white font-bold mb-3 text-lg">เป้าหมาย</h4>
                <p class="text-slate-400 leading-relaxed text-base">
                  มีความมุ่งมั่นที่จะพัฒนาตนเองสู่บทบาท <span class="text-white font-medium">Full-stack Developer</span> อย่างเต็มตัว 
                  โดยอาศัยพื้นฐานจากการเป็น Automation Engineer มาต่อยอด และพร้อมที่จะเรียนรู้เทคโนโลยีใหม่ ๆ เพื่อส่งมอบคุณค่าและนวัตกรรมที่ยั่งยืนให้แก่ทีมและองค์กร
                </p>
              </div>
            </div>

            <div class="flex flex-wrap gap-4 pt-4">
              <a href="Thanatchaya-Resume.pdf" target="_blank"
                class="px-8 py-3 bg-cyan-500 text-slate-900 font-bold rounded-lg hover:bg-cyan-400 transition-all duration-300 shadow-[0_5px_15px_rgba(6,182,212,0.2)]">
                VIEW RESUME
              </a>
              <a href="transcript.pdf" target="_blank"
                class="px-8 py-3 border border-slate-700 text-slate-300 font-bold rounded-lg hover:border-cyan-400 hover:text-cyan-400 transition-all duration-300">
                TRANSCRIPT
              </a>
            </div>

          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
@keyframes pulse-slow {
  0%, 100% { opacity: 0.2; transform: scale(1); }
  50% { opacity: 0.4; transform: scale(1.1); }
}

@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-6px); }
}

.animate-pulse-slow { animation: pulse-slow 10s ease-in-out infinite; }
.animate-float { animation: float 4s ease-in-out infinite; }

/* ทำให้ฟอนต์อ่านง่ายขึ้นในพื้นหลังมืด */
.container {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>