<template>
    <section id="contact" class="w-full py-24 px-6 border-t-2 border-slate-200 dark:border-white/10 bg-white/50 dark:bg-black/40 backdrop-blur-xl transition-colors duration-300">
        <div class="max-w-6xl mx-auto grid md:grid-cols-2 gap-12">

            <!-- LEFT SIDE -->
            <div class="space-y-6">
                <p class="text-indigo-600 dark:text-cyan-400 tracking-[0.3em] text-sm font-bold transition-colors duration-300">
                    CONTACT
                </p>

                <h2 class="text-4xl md:text-5xl font-black text-slate-900 dark:text-white leading-tight transition-colors duration-300">
                    LET’S CONNECT
                </h2>

                <p class="text-slate-600 dark:text-gray-400 leading-relaxed transition-colors duration-300 font-medium">
                    Feel free to contact me for collaboration, internship
                    opportunities, projects, or just to connect and chat
                    about web development and design.
                </p>

                <!-- SOCIAL LINKS -->
                <div class="space-y-4 pt-4">

                    <a href="https://mail.google.com/"
                        class="flex items-center justify-between border-2 border-slate-200 shadow-md shadow-slate-300/60 dark:border-white/10 bg-white/90 dark:bg-black/20 p-4 hover:-translate-y-1 hover:border-cyan-400 hover:shadow-sm hover:shadow-cyan-300/30 dark:hover:bg-white/5 dark:shadow-none transition-all duration-300 group">
                        <div>
                            <p class="text-slate-500 font-bold font-mono text-sm">EMAIL</p>
                            <p class="text-slate-900 font-bold dark:text-white group-hover:text-cyan-600 dark:group-hover:text-cyan-400 transition-colors duration-300">
                                poylnwza123@gmail.com
                            </p>
                        </div>

                        <span class="text-cyan-600 font-bold dark:text-cyan-400 transition-colors duration-300">↗</span>
                    </a>

                    <a href="https://github.com/Thitiratss" target="_blank"
                        class="flex items-center justify-between border-2 border-slate-200 shadow-md shadow-slate-300/60 dark:border-white/10 bg-white/90 dark:bg-black/20 p-4 hover:-translate-y-1 hover:border-cyan-400 hover:shadow-md hover:shadow-cyan-400/50 dark:hover:bg-white/5 dark:shadow-none transition-all duration-300 group">
                        <div>
                            <p class="text-slate-500 font-bold font-mono text-sm">GITHUB</p>
                            <p class="text-slate-900 font-bold dark:text-white group-hover:text-cyan-600 dark:group-hover:text-cyan-400 transition-colors duration-300">
                                github.com/Thitiratss
                            </p>
                        </div>

                        <span class="text-cyan-600 font-bold dark:text-cyan-400 transition-colors duration-300">↗</span>
                    </a>

                    <a href="https://linkedin.com" target="_blank"
                        class="flex items-center justify-between border-2 border-slate-200 shadow-md shadow-slate-300/60 dark:border-white/10 bg-white/90 dark:bg-black/20 p-4 hover:-translate-y-1 hover:border-cyan-400 hover:shadow-md hover:shadow-cyan-400/50 dark:hover:bg-white/5 dark:shadow-none transition-all duration-300 group">
                        <div>
                            <p class="text-slate-500 font-bold font-mono text-sm">LINKEDIN</p>
                            <p class="text-slate-900 font-bold dark:text-white group-hover:text-cyan-600 dark:group-hover:text-cyan-400 transition-colors duration-300">
                                linkedin.com/Thitiratss
                            </p>
                        </div>

                        <span class="text-cyan-600 font-bold dark:text-cyan-400 transition-colors duration-300">↗</span>
                    </a>

                </div>
            </div>

            <!-- RIGHT SIDE -->
            <div
                class="border-2 border-indigo-100 shadow-xl shadow-indigo-200/60 dark:border-white/10 bg-white/90 dark:bg-black/30 backdrop-blur-2xl p-8 space-y-6 transition-all duration-300 hover:border-indigo-400 hover:shadow-2xl hover:shadow-indigo-400/50 dark:hover:border-cyan-400/40 dark:shadow-none dark:hover:shadow-xl dark:hover:shadow-cyan-400/20">

                <h3 class="text-2xl font-bold text-indigo-900 dark:text-white font-mono transition-colors duration-300">
                    SEND MESSAGE
                </h3>

                <form class="space-y-5">

                    <!-- NAME -->
                    <div class="space-y-2">
                        <label class="text-sm font-bold text-slate-600 dark:text-gray-400 transition-colors duration-300">
                            YOUR NAME <span class="text-pink-500 dark:text-red-400">*</span>
                        </label>

                        <input type="text" placeholder="Enter your name"
                            class="w-full border-2 border-slate-200 dark:border-white/10 bg-slate-50 dark:bg-black/20 px-4 py-3 text-slate-900 dark:text-white outline-none focus:border-indigo-400 focus:shadow-md focus:shadow-indigo-400/30 dark:focus:shadow-none dark:focus:border-cyan-400 transition-all duration-300 font-medium" />
                    </div>

                    <!-- EMAIL -->
                    <div class="space-y-2">
                        <label class="text-sm font-bold text-slate-600 dark:text-gray-400 transition-colors duration-300">
                            YOUR EMAIL <span class="text-pink-500 dark:text-red-400">*</span>
                        </label>

                        <input type="email" placeholder="Enter your email"
                            class="w-full border-2 border-slate-200 dark:border-white/10 bg-slate-50 dark:bg-black/20 px-4 py-3 text-slate-900 dark:text-white outline-none focus:border-indigo-400 focus:shadow-md focus:shadow-indigo-400/30 dark:focus:shadow-none dark:focus:border-cyan-400 transition-all duration-300 font-medium" />
                    </div>

                    <!-- MESSAGE -->
                    <div class="space-y-2">
                        <label class="text-sm font-bold text-slate-600 dark:text-gray-400 transition-colors duration-300">
                            MESSAGE <span class="text-pink-500 dark:text-red-400">*</span>
                        </label>
                        <textarea rows="6" placeholder="Write your message..."
                            class="w-full border-2 border-slate-200 dark:border-white/10 bg-slate-50 dark:bg-black/20 px-4 py-3 text-slate-900 dark:text-white outline-none resize-none focus:border-indigo-400 focus:shadow-md focus:shadow-indigo-400/30 dark:focus:shadow-none dark:focus:border-cyan-400 transition-all duration-300 font-medium"></textarea>
                    </div>

                    <!-- BUTTON -->
                    <button type="submit"
                        class="w-full border-2 border-indigo-500 dark:border-cyan-400 bg-indigo-50 dark:bg-cyan-400/10 py-3 text-indigo-700 dark:text-cyan-400 font-bold tracking-widest hover:bg-indigo-500 hover:text-white hover:shadow-md hover:shadow-indigo-400/40 active:shadow-none active:translate-y-1 dark:hover:bg-cyan-400 dark:hover:text-black dark:hover:shadow-none dark:active:translate-y-0 transition-all duration-300">
                        SEND MESSAGE
                    </button>

                </form>
            </div>
        </div>
    </section>
</template>