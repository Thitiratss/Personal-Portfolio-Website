<template>
  <footer class="w-full border-t-2 border-indigo-100 dark:border-white/10 py-10 mt-20 bg-gradient-to-r from-blue-50 via-indigo-50 to-purple-50 dark:bg-black/90 dark:bg-none backdrop-blur-xl transition-colors duration-500">

    <!-- NAV LINKS -->
    <div class="flex flex-wrap justify-center gap-4 sm:gap-8 mb-6 text-xs sm:text-sm font-mono font-bold px-4">
      <a href="#profile" class="text-indigo-900 dark:text-white hover:text-pink-600 dark:hover:text-cyan-300 transition-colors duration-300">PROFILE</a>
      <a href="#skills" class="text-indigo-900 dark:text-white hover:text-pink-600 dark:hover:text-cyan-300 transition-colors duration-300">SKILLS</a>
      <a href="#projects" class="text-indigo-900 dark:text-white hover:text-pink-600 dark:hover:text-cyan-300 transition-colors duration-300">PROJECTS</a>
      <a href="#experience" class="text-indigo-900 dark:text-white hover:text-pink-600 dark:hover:text-cyan-300 transition-colors duration-300">EXPERIENCE</a>
      <a href="#contact" class="text-indigo-900 dark:text-white hover:text-pink-600 dark:hover:text-cyan-300 transition-colors duration-300">CONTACT</a>
    </div>

    <!-- SOCIAL LINKS -->
    <div class="flex justify-center gap-8 text-indigo-600 dark:text-cyan-200 transition-colors duration-300">

      <!-- GitHub -->
      <a
        href="https://github.com/Thitiratss"
        target="_blank"
        class="hover:text-pink-500 dark:hover:text-cyan-300 hover:-translate-y-1 transition-all duration-300 p-2"
      >
        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 sm:w-5 sm:h-5" fill="currentColor" viewBox="0 0 24 24">
          <path d="M12 .5C5.73.5.75 5.6.75 11.9c0 5.1 3.29 9.45 7.86 10.98.58.1.79-.26.79-.57v-2.1c-3.2.7-3.87-1.4-3.87-1.4-.53-1.4-1.3-1.7-1.3-1.7-1.06-.75.08-.73.08-.73 1.17.08 1.79 1.2 1.79 1.2 1.04 1.8 2.73 1.3 3.4 1 .1-.8.4-1.3.73-1.6-2.55-.3-5.23-1.3-5.23-5.8 0-1.3.45-2.4 1.2-3.3-.12-.3-.52-1.6.12-3.3 0 0 1-.3 3.3 1.2a11 11 0 0 1 6 0c2.3-1.5 3.3-1.2 3.3-1.2.64 1.7.24 3 .12 3.3.75.9 1.2 2 1.2 3.3 0 4.5-2.7 5.5-5.3 5.8.4.3.77 1 .77 2.1v3.1c0 .3.2.67.8.57A11.2 11.2 0 0 0 23.25 11.9C23.25 5.6 18.27.5 12 .5z"/>
        </svg>
      </a>

      <!-- Email -->
      <a href="mailto:youremail@gmail.com" class="hover:text-pink-500 dark:hover:text-cyan-300 hover:-translate-y-1 transition-all duration-300 p-2">
        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 sm:w-5 sm:h-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            d="M3 8l9 6 9-6M3 8a2 2 0 012-2h14a2 2 0 012 2M3 8v8a2 2 0 002 2h14a2 2 0 002-2V8" />
        </svg>
      </a>

      <!-- LinkedIn -->
      <a href="https://linkedin.com" target="_blank" class="hover:text-pink-500 dark:hover:text-cyan-300 hover:-translate-y-1 transition-all duration-300 p-2">
        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 sm:w-5 sm:h-5" fill="currentColor" viewBox="0 0 24 24">
          <path d="M4.98 3.5C4.98 4.88 3.87 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1 4.98 2.12 4.98 3.5zM0 24h5V7H0v17zM8 7h4.8v2.3h.1c.7-1.3 2.4-2.7 5-2.7 5.3 0 6.3 3.5 6.3 8V24h-5v-9.5c0-2.3 0-5.2-3.2-5.2s-3.7 2.5-3.7 5V24H8V7z"/>
        </svg>
      </a>

    </div>

  </footer>
</template>