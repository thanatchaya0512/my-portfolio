<template>
  <section id="skills" class="min-h-screen bg-[#171616] py-28 relative overflow-hidden">
    <div class="absolute top-0 right-0 w-96 h-96 bg-cyan-500/5 rounded-full blur-[120px] -z-0"></div>

    <div class="container mx-auto px-6 relative z-10">
      <div class="max-w-6xl mx-auto mb-20">
        <h2 class="text-4xl md:text-5xl font-bold text-white mb-2 flex items-center group">
          <span class="text-cyan-400 font-mono text-xl mr-4 opacity-80">04.</span>
          <span class="group-hover:text-cyan-400 transition-colors duration-300 uppercase">Skills & Tech Stack</span>
          <div class="hidden md:block h-[1px] flex-1 max-w-xs bg-slate-700 ml-8"></div>
        </h2>
        <p class="text-slate-300 font-mono text-sm uppercase tracking-[0.2em] ml-12">ทักษะและเครื่องมือที่ใช้ในการพัฒนาแบ่งตามหมวดหมู่</p>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 max-w-6xl mx-auto">
        
        <div class="lg:col-span-8 space-y-12">
          
          <div class="space-y-6">
            <h3 class="text-cyan-400 font-mono text-lg flex items-center gap-3">
              <span class="text-slate-500 font-sans">#</span> Languages
            </h3>
            <div class="grid grid-cols-3 sm:grid-cols-6 gap-4">
              <div v-for="skill in languages" :key="skill.name" 
                class="flex flex-col items-center p-3 bg-slate-800/20 border border-slate-700/50 rounded-xl hover:border-cyan-400/40 hover:-translate-y-1 transition-all duration-300 group">
                <img :src="skill.icon" :alt="skill.name" class="w-10 h-10 mb-2 md:grayscale group-hover:grayscale-0 transition-all duration-300">
                <span class="text-slate-400 group-hover:text-white text-[10px] font-medium uppercase tracking-tighter text-center">{{ skill.name }}</span>
              </div>
            </div>
          </div>

          <div class="space-y-6">
            <h3 class="text-cyan-400 font-mono text-lg flex items-center gap-3">
              <span class="text-slate-500 font-sans">#</span> Frameworks & Runtimes
            </h3>
            <div class="grid grid-cols-3 sm:grid-cols-5 gap-4">
              <div v-for="skill in frameworks" :key="skill.name" 
                class="flex flex-col items-center p-3 bg-slate-800/20 border border-slate-700/50 rounded-xl hover:border-cyan-400/40 hover:-translate-y-1 transition-all duration-300 group">
                <img :src="skill.icon" :alt="skill.name" class="w-10 h-10 mb-2 md:grayscale group-hover:grayscale-0 transition-all duration-300">
                <span class="text-slate-400 group-hover:text-white text-[10px] font-medium uppercase tracking-tighter text-center">{{ skill.name }}</span>
              </div>
            </div>
          </div>

          <div class="space-y-6">
            <h3 class="text-cyan-400 font-mono text-lg flex items-center gap-3">
              <span class="text-slate-500 font-sans">#</span> Libraries & UI Components
            </h3>
            <div class="grid grid-cols-3 sm:grid-cols-5 gap-4">
              <div v-for="skill in libraries" :key="skill.name" 
                class="flex flex-col items-center p-3 bg-slate-800/20 border border-slate-700/50 rounded-xl hover:border-cyan-400/40 hover:-translate-y-1 transition-all duration-300 group">
                <img :src="skill.icon" :alt="skill.name" class="w-10 h-10 mb-2 md:grayscale group-hover:grayscale-0 transition-all duration-300 object-contain">
                <span class="text-slate-400 group-hover:text-white text-[10px] font-medium uppercase tracking-tighter text-center">{{ skill.name }}</span>
              </div>
            </div>
          </div>

          <div class="space-y-6">
            <h3 class="text-cyan-400 font-mono text-lg flex items-center gap-3">
              <span class="text-slate-500 font-sans">#</span> Dev Tools & Design
            </h3>
            <div class="grid grid-cols-3 sm:grid-cols-6 gap-4">
              <div v-for="skill in devToolsIcons" :key="skill.name" 
                class="flex flex-col items-center p-3 bg-slate-800/20 border border-slate-700/50 rounded-xl hover:border-cyan-400/40 hover:-translate-y-1 transition-all duration-300 group">
                <img :src="skill.icon" :alt="skill.name" class="w-10 h-10 mb-2 md:grayscale group-hover:grayscale-0 transition-all duration-300 object-contain">
                <span class="text-slate-400 group-hover:text-white text-[10px] font-medium uppercase tracking-tighter text-center">{{ skill.name }}</span>
              </div>
            </div>
          </div>
        </div>

        <div class="lg:col-span-4 space-y-12">
          
          <div class="space-y-6">
            <h3 class="text-cyan-400 font-mono text-xl flex items-center gap-3">
              <span class="text-slate-500 font-sans">#</span> Databases & Data
            </h3>
            <div class="flex flex-wrap gap-2">
              <div v-for="tool in databaseTools" :key="tool"
                class="px-3 py-1.5 bg-slate-800/40 border border-slate-700/50 rounded-lg text-slate-400 text-xs hover:text-cyan-400 hover:border-cyan-400/50 hover:bg-cyan-400/5 transition-all cursor-default">
                {{ tool }}
              </div>
            </div>
          </div>

          <div class="space-y-6">
            <h3 class="text-cyan-400 font-mono text-xl flex items-center gap-3">
              <span class="text-slate-500 font-sans">#</span> Soft Skills
            </h3>
            <div class="flex flex-col gap-3">
              <div v-for="soft in softSkills" :key="soft"
                class="flex items-center gap-3 p-3 bg-slate-800/10 border-l-2 border-slate-700 hover:border-cyan-400 hover:bg-slate-800/30 transition-all text-slate-400 text-sm group">
                <span class="text-cyan-400 group-hover:translate-x-1 transition-transform">▹</span> {{ soft }}
              </div>
            </div>
          </div>

        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// 1. Languages
const languages = [
  { name: 'TypeScript', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg' },
  { name: 'JavaScript', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg' },
  { name: 'Python', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg' },
  { name: 'PHP', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-original.svg' },
  { name: 'HTML5', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg' },
  { name: 'CSS3', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg' },
];

// 2. Frameworks & Runtimes
const frameworks = [
  { name: 'Vue.js', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg' },
  { name: 'Node.js', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg' },
  { name: 'FastAPI', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/fastapi/fastapi-original.svg' },
  { name: 'Laravel', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/laravel/laravel-original.svg' },
  { name: 'Django', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/django/django-plain.svg' },
];

// 3. Libraries & UI
const libraries = [
  { name: 'Ant Design Vue', icon: 'https://gw.alipayobjects.com/zos/rmsportal/KDpgvguMpGfqaHPjicRK.svg' },
  { name: 'ApexCharts', icon: 'https://apexcharts.com/media/apexcharts-logo.png' },
  { name: 'OpenCV', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/opencv/opencv-original.svg' },
  { name: 'Socket.io', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/socketio/socketio-original.svg' },
  { name: 'Axios', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/axios/axios-plain.svg' },
];

// 4. Dev Tools & Design (New Icon Category)
const devToolsIcons = [
  { name: 'Docker', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg' },
  { name: 'GitLab', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/gitlab/gitlab-original.svg' },
  { name: 'Postman', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postman/postman-original.svg' },
  { name: 'XAMPP', icon: 'https://cdn.simpleicons.org/xampp/FB7A24' },
  { name: 'Bootstrap', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg' },
  { name: 'Figma', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/figma/figma-original.svg' },
];

// 5. Databases & Data Analytics (Tag format)
const databaseTools = [
  'MySQL', 'MariaDB', 'PostgreSQL', 'MongoDB',
  'DBeaver', 'Power BI', 'Looker Studio',
  'Orange Data Mining', 'Balsamiq', 'Excel'
];

// 6. Soft Skills
const softSkills = [
  'ทักษะการทำงานเป็นทีม', 'ทักษะการเรียนรู้เร็ว',
  'ทักษะการสื่อสาร', 'ทักษะความสัมพันธ์ระหว่างบุคคล',
  'ทักษะการบริหารเวลา', 'ทักษะการแก้ปัญหา'
];
</script>

<style scoped>
.transition-all {
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
}
</style>