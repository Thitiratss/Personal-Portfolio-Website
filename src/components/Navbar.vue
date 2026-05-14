<script setup>
import { inject, ref } from 'vue'

const { isDark, toggleTheme } = inject('theme')
const isMobileMenuOpen = ref(false)

const toggleMobileMenu = () => {
  isMobileMenuOpen.value = !isMobileMenuOpen.value
}
</script>

<template>
  <nav class="fixed top-0 w-full z-50 flex items-center justify-between md:justify-start px-6 py-4 backdrop-blur-xl bg-white/80 dark:bg-surface/80 border-b border-gray-200 dark:border-white/20 transition-colors duration-300">
    
    <!-- Desktop Menu -->
    <div class="hidden md:flex gap-9 ml-20 flex-1 font-mono">
      <a href="#profile" class="text-gray-600 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">PROFILE</a>
      <a href="#skills" class="text-gray-600 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">SKILLS</a>
      <a href="#experience" class="text-gray-600 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">EXPERIENCE</a>
      <a href="#projects" class="text-gray-600 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">PROJECTS</a>
      <a href="#contact" class="text-gray-600 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">CONTACT</a>
    </div>

    <!-- Theme Toggle -->
    <button @click="toggleTheme" class="ml-auto md:ml-0 md:mr-6 p-2 rounded-full hover:bg-gray-200 dark:hover:bg-white/10 transition-colors flex items-center justify-center">
      <span v-if="isDark" class="material-symbols-outlined text-yellow-500 dark:text-yellow-300 text-[24px]">light_mode</span>
      <span v-else class="material-symbols-outlined text-gray-700 text-[24px]">dark_mode</span>
    </button>

    <!-- Mobile Menu Toggle -->
    <div class="md:hidden flex items-center"> 
      <button @click="toggleMobileMenu" class="p-2 flex items-center justify-center text-cyan-600 dark:text-primary-fixed">
        <span class="material-symbols-outlined">{{ isMobileMenuOpen ? 'close' : 'menu' }}</span>
      </button>
    </div>

    <!-- Mobile Menu Dropdown -->
    <div v-if="isMobileMenuOpen" class="absolute top-[100%] left-0 w-full bg-white dark:bg-surface border-b border-gray-200 dark:border-white/20 md:hidden flex flex-col p-4 shadow-lg transition-colors duration-300">
      <a @click="toggleMobileMenu" href="#profile" class="py-3 text-gray-800 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">PROFILE</a>
      <a @click="toggleMobileMenu" href="#skills" class="py-3 text-gray-800 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">SKILLS</a>
      <a @click="toggleMobileMenu" href="#experience" class="py-3 text-gray-800 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">EXPERIENCE</a>
      <a @click="toggleMobileMenu" href="#projects" class="py-3 text-gray-800 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">PROJECTS</a>
      <a @click="toggleMobileMenu" href="#contact" class="py-3 text-gray-800 dark:text-on-surface-variant hover:text-cyan-600 dark:hover:text-primary-fixed transition-colors">CONTACT</a>
    </div>
  </nav>
</template>