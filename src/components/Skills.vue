<script setup>
const skills = [
  "UI/UX",
  "Figma",

  "Vue.js",
  "JavaScript",
  "Tailwind",
  "Node.js",

  "Java",
  "SQL",
  "Git",

  "Basic DevOps"
]
</script>

<template>
  <section class="mb-32">
    <h3 class="text-purple-600 dark:text-cyan-300 text-2xl mb-8 font-mono font-bold transition-colors duration-300" id="skills">
      TECH_SKILLS [tools]
    </h3>

    <div class="grid grid-cols-2 md:grid-cols-4 gap-4">

      <div
        v-for="(skill, i) in skills"
        :key="i"
        class="group relative p-4 text-center border-2 border-slate-200 shadow-md shadow-slate-300/60 dark:border-white/10 overflow-hidden
               bg-white/90 dark:bg-black/20 backdrop-blur-md
               transition-all duration-300
               hover:-translate-y-1 hover:border-pink-400 hover:shadow-lg hover:shadow-pink-400/60 dark:hover:border-cyan-400/40 dark:shadow-none dark:hover:shadow-cyan-100"
      >

        <!-- glow -->
        <div
          class="absolute inset-0 opacity-0 group-hover:opacity-100
                 transition duration-500 
                 bg-gradient-to-br from-pink-50 to-purple-50 dark:bg-cyan-400/10"></div>

        <!-- text -->
        <span
          class="relative z-10 text-slate-700 dark:text-gray-300 font-bold font-mono
                 transition duration-300
                 group-hover:text-pink-600 dark:group-hover:text-cyan-200"
        >
          {{ skill }}
        </span>

      </div>

    </div>
  </section>
</template>

