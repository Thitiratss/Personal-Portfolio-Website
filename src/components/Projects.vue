<script setup>
import kinraidee from "@/assets/kinraidee.png"
import Intgerated from "@/assets/Intgerated.png"
import hellowordproject from "@/assets/hellowordproject.png"

const projects = [
    {
        title: "KINRAIDEE",
        description: "Restaurant recommendation website UI/UX project.",
        image: kinraidee,
        link: "https://int-250-g04-spongebob-kinraidee.vercel.app/"
    },
    {
        title: "INTEGRATED PROJECT",
        description: "Second-year integrated web development project.",
        image: Intgerated,
        link: "https://github.com/"
    },
    {
        title: "HELLO WORLD PROJECT",
        description: "First-year project focused on UI/UX design.",
        image: hellowordproject,
        link: "https://www.figma.com/proto/ggjWib8bGJBn4ujhGlyry8/sit-hello-world?node-id=142-605&starting-point-node-id=142%3A605&t=L3qbtMf29XIUkH5y-1"
    }
]
</script>

<template>
    <section id="projects" class="mb-32">

        <h3 class="text-pink-600 dark:text-pink-300 text-2xl mb-8 font-mono font-bold transition-colors duration-300">
            PROJECTS
        </h3>

        <div class="grid md:grid-cols-3 gap-6">

            <div v-for="(project, i) in projects" :key="i"
                class="bg-white/90 border-2 border-indigo-100 shadow-md shadow-indigo-200/60 dark:border-white/10 dark:bg-black/20 overflow-hidden
                transition-all duration-500 hover:-translate-y-2 hover:border-cyan-400 hover:shadow-lg hover:shadow-cyan-400/50 dark:hover:border-cyan-400/40 dark:shadow-none dark:hover:shadow-cyan-100 dark:hover:bg-black/40">

                <!-- IMAGE -->
                <img :src="project.image"
                    class="w-full h-48 object-cover border-b-2 border-indigo-50 dark:border-white/10" alt="" />

                <!-- CONTENT -->
                <div class="p-5">

                    <h4 class="text-indigo-900 dark:text-white font-bold font-mono mb-2 transition-colors duration-300">
                        {{ project.title }}
                    </h4>

                    <p
                        class="text-slate-600 dark:text-gray-400 text-sm mb-6 transition-colors duration-300 font-medium">
                        {{ project.description }}
                    </p>

                    <!-- BUTTON -->
                    <a :href="project.link" target="_blank" class="inline-block px-4 py-2 border-2 border-cyan-500 dark:border border-cyan-300
                   text-cyan-600 dark:text-cyan-300 text-sm font-bold font-mono shadow-sm shadow-cyan-500/30 hover:shadow-none hover:translate-y-[3px] hover:bg-cyan-500 hover:text-white dark:shadow-none dark:hover:bg-cyan-300/10 dark:hover:translate-y-0 dark:hover:text-cyan-300
                   transition-all duration-300">
                        VIEW_PROJECT
                    </a>

                </div>

            </div>

        </div>

    </section>
</template>