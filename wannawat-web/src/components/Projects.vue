<script setup>
const projects = [
    { id: 1, title: "Job Search Website", link: "https://github.com/navysingchai/INT250-Project.git", tools: ["Vue.js", "Tailwind CSS"] },
    { id: 2, title: "Blind Timer Game", link: "https://github.com/navysingchai/INT250-Game-Project-007xGroup.git", tools: ["Vue.js", "Tailwind CSS"] },
    { id: 3, title: "CureX", link: "https://github.com/UltraPixel042/int250-workshop-05.git", tools: ["Vue.js", "Tailwind CSS"] },
    { id: 4, title: "Lab / Exercises", link: "https://github.com/UltraPixel042/int250-67130500036-Wannawat.git", tools: ["Vue.js", "Tailwind CSS"] },
    { id: 5, title: "Integrated Projected", link: "https://github.com/IT-BANGMOD-INTEGRATED-PROJECT-2025/intproj25-SY2.git", tools: ["JavaScript", "Tailwind CSS"] },
]
</script>

<template>
    <section
        class="flex flex-col gap-6 border-b border-slate-200 dark:border-slate-700 shadow-xs px-6 lg:px-18 py-6 lg:py-12"
        id="projects">

        <h2 class="text-xl font-medium text-slate-700 dark:text-slate-200">Projects</h2>

        <div
            class="flex flex-col border border-slate-200 dark:border-slate-700 rounded-2xl overflow-hidden divide-y divide-slate-200 dark:divide-slate-700">
            <div class="flex justify-between items-center gap-3 px-4 py-3 w-full" v-for="project in projects">

                <div class="flex flex-col items-start gap-2">
                    <a :href="project.link" target="_blank" rel="noopener noreferrer" class="hover:text-indigo-500 dark:hover:text-indigo-400">{{ project.title }}</a>
                    <div class="flex">
                        <span class="border border-slate-200 dark:border-slate-700 py-0.5 px-2 rounded-2xl text-sm w-fit"
                            v-for="tool in project.tools" :key="tool">
                            {{ tool }}
                        </span>
                    </div>
                </div>
                <a :href="project.link" target="_blank" rel="noopener noreferrer">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor"
                        class="bi bi-box-arrow-up-right border-2 dark:border border-slate-200 dark:border-slate-500 p-1 rounded-lg shadow-lg text-slate-500 dark:text-slate-300 hover:text-indigo-500 dark:hover:text-indigo-400"
                        viewBox="0 0 16 16">
                        <path fill-rule="evenodd"
                            d="M8.636 3.5a.5.5 0 0 0-.5-.5H1.5A1.5 1.5 0 0 0 0 4.5v10A1.5 1.5 0 0 0 1.5 16h10a1.5 1.5 0 0 0 1.5-1.5V7.864a.5.5 0 0 0-1 0V14.5a.5.5 0 0 1-.5.5h-10a.5.5 0 0 1-.5-.5v-10a.5.5 0 0 1 .5-.5h6.636a.5.5 0 0 0 .5-.5" />
                        <path fill-rule="evenodd"
                            d="M16 .5a.5.5 0 0 0-.5-.5h-5a.5.5 0 0 0 0 1h3.793L6.146 9.146a.5.5 0 1 0 .708.708L15 1.707V5.5a.5.5 0 0 0 1 0z" />
                    </svg>
                </a>

            </div>
        </div>

    </section>
</template>

<style scoped></style>
