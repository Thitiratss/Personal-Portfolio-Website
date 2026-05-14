<script setup>
import { ref, onMounted, provide } from 'vue';
import Hero from "./components/Hero.vue";
import Skills from "@/components/Skills.vue"
import AboutMe from "@/components/AboutMe.vue"
import Experience from "@/components/Experience.vue";
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";

const isDark = ref(false);

const toggleTheme = () => {
  isDark.value = !isDark.value;
  if (isDark.value) {
    document.documentElement.classList.add('dark');
    localStorage.setItem('theme', 'dark');
  } else {
    document.documentElement.classList.remove('dark');
    localStorage.setItem('theme', 'light');
  }
};

provide('theme', { isDark, toggleTheme });

onMounted(() => {
  const savedTheme = localStorage.getItem('theme');
  if (savedTheme === 'dark' || (!savedTheme && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
    isDark.value = true;
    document.documentElement.classList.add('dark');
  } else {
    isDark.value = false;
    document.documentElement.classList.remove('dark');
  }
});
</script>

<template>
  <div class="min-h-screen bg-[radial-gradient(ellipse_at_top,_var(--tw-gradient-stops))] from-blue-50 via-slate-50 to-purple-50 dark:bg-none dark:bg-background text-slate-800 dark:text-white transition-colors duration-500">
    <Navbar />

    <main>
      <div class="max-w-6xl mx-auto px-6">
        <Hero />
        <AboutMe />
        <Skills/>
        <Experience />
        <Projects />
        <Contact />
      </div>
    </main>

    <Footer />
  </div>
</template>

<style scoped></style>