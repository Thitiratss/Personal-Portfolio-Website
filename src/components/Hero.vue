<script setup>
import me from "@/assets/me.png"
</script>

<template>

  <main class="pt-24 px-6 max-w-6xl mx-auto w-full">

    <!-- HERO -->
    <section class="flex flex-col-reverse lg:flex-row items-center gap-10 min-h-[80vh] mb-32">

      <!-- TEXT -->
      <div class="lg:w-7/12 space-y-6" id="profile">
        <h1
          class="text-5xl md:text-7xl font-bold text-indigo-700 dark:text-cyan-300 leading-tight transition-colors duration-300">
          THITIRAT<br />SRITHOMYA
        </h1>

        <h2
          class="text-xl border-l-4 border-pink-500 dark:border-pink-400 pl-4 text-pink-600 dark:text-pink-300 transition-colors duration-300 font-bold">
          IT STUDENT
        </h2>

        <p class="text-slate-700 dark:text-gray-300 max-w-xl transition-colors duration-300 text-lg">
          An Information Technology second-year student from King Mongkut’s University of Technology Thonburi
        </p>

        <div class="flex justify-center md:justify-start gap-8 flex-wrap pt-4">
          <button
            class="px-6 py-3 bg-cyan-500 text-white font-bold transition-all duration-300  hover:translate-y-1 hover:bg-cyan-600 dark:bg-cyan-300 dark:text-black  dark:hover:scale-95 dark:hover:translate-y-0">
            VIEW PROJECTS
          </button>

          <button
            class="px-6 py-3 border-2 border-purple-500 text-purple-600 font-bold transition-all duration-300  hover:translate-y-1 hover:bg-purple-50 dark:border-cyan-300 dark:text-cyan-300  dark:hover:bg-cyan-300/10 dark:hover:translate-y-0 border border-cyan-600">
            CONTACT.EXE
          </button>
        </div>

      </div>

      <div class="lg:w-5/12 flex justify-center lg:justify-end">

        <div class="retro-border bg-surface-container-low border-2 border-transparent shadow-2xl hover:shadow-cyan-500/50 overflow-hidden relative window-shadow w-[280px] sm:w-[320px] lg:w-[340px]
          hover:-translate-y-2 duration-500 transition-all">

          <!-- Title Bar -->
          <div
            class="px-3 py-2 flex justify-between items-center bg-transparent transition-colors duration-300">
            <div class="flex items-center gap-2">
              <span class="text-white text-xs transition-colors duration-300">👤</span>
              <span
                class="text-white text-xs font-mono font-bold uppercase transition-colors duration-300">PORTRAIT.EXE</span>
            </div>
          </div>

          <!-- IMAGE -->
          <div class="bg-white p-3">
            <img :src="me"
              class="w-full h-[320px] sm:h-[380px] lg:h-[420px] object-cover border-2 border-black/10" />
          </div>

        </div>

      </div>

    </section>

  </main>

</template>

<style></style>