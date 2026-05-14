<script setup>
const experiences = [
    {
        year: "2025",
        color: "text-pink-600 dark:text-pink-300",
        title: "INTEGRATED PROJECT",
        description:
            "Worked on a second-year integrated project focused on teamwork and web development."
    },

    {
        year: "2025",
        color: "text-cyan-600 dark:text-cyan-300",
        title: "APPLIED LEARNING PROGRAM",
        description:
            "Participated in the KMUTT Applied Learning 2 employment program during June – July 2025."
    },

    {
        year: "2024",
        color: "text-purple-600 dark:text-yellow-300",
        title: "HELLO WORLD PROJECT",
        description:
            "Contributed as a UI/UX designer for the HelloWorld project during first year, second semester."
    }
]
</script>

<template>
    <section id="experience" class="mb-32">

        <h3 class="text-cyan-600 dark:text-cyan-300 text-2xl mb-8 font-mono font-bold transition-colors duration-300">
            EXPERIENCE_LOG
        </h3>

        <div
            class="bg-white/90 border-2 border-purple-100 shadow-md shadow-purple-200/60 dark:border-white/10 dark:bg-black/20 p-6 space-y-6 transition-all duration-500 hover:-translate-y-2 hover:border-purple-400 hover:shadow-lg hover:shadow-purple-400/40 dark:hover:border-cyan-400/40 dark:shadow-none dark:hover:shadow-cyan-100 dark:hover:bg-black/40">
            <div v-for="(item, i) in experiences" :key="i" class="flex gap-4">

                <span class="font-mono font-bold transition-colors duration-300" :class="item.color">
                    [{{ item.year }}]
                </span>

                <div>
                    <h4 class="text-slate-900 dark:text-white font-bold font-mono transition-colors duration-300">
                        {{ item.title }}
                    </h4>

                    <p class="text-slate-600 dark:text-gray-400 text-sm transition-colors duration-300 font-medium">
                        {{ item.description }}
                    </p>
                </div>

            </div>

        </div>

    </section>
</template>