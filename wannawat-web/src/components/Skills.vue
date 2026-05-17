<script setup>

const frontend = [
    { id: 1, name: "Vue.js", length: 40, color: "#3fbef6" },
    { id: 2, name: "Tailwind CSS", length: 70, color: "#3fbef6" },
    { id: 3, name: "TypeScript", length: 20, color: "#377cc8" },
    { id: 4, name: "HTML/CSS", length: 80, color: "#e5532d" },
]

const tools = [
    { id: 1, name: "Node.js", length: 25, color: "#7bb862" },
    { id: 2, name: "Git / GitHub", length: 75, color: "#f05639" },
    { id: 3, name: "Canva", length: 85, color: "#a259ff" },
    { id: 4, name: "Power BI", length: 20, color: "#f2c811" },
]

</script>

<template>
    <section
        class="flex flex-col gap-6 border-b border-slate-200 dark:border-slate-700 shadow-xs px-6 lg:px-18 py-6 lg:py-12"
        id="skills">

        <h2 class="text-xl font-medium text-slate-700 dark:text-slate-200">Skills</h2>

        <div class="flex flex-col md:flex-row gap-6 md:gap-15">

            <!-- Frontend -->
            <div class="flex flex-col gap-1 text-sm w-full">
                <span class="font-medium text-slate-500 dark:text-slate-400 mb-1">Frontend</span>
                <div>
                    <div class="flex items-center gap-1 my-2 w-full" v-for="item in frontend" :key="item.id">
                        <span class="min-w-24 truncate text-slate-700 dark:text-slate-200">{{ item.name }}</span>
                        <div
                            class="flex-1 h-2 bg-slate-100 dark:bg-slate-700 rounded-full overflow-hidden border border-slate-200 dark:border-slate-600">
                            <div class="h-full rounded-full transition-all duration-500"
                                :style="{ background: item.color, width: item.length + '%' }"></div>
                        </div>
                        <span class="w-8 text-right text-slate-500 dark:text-slate-400">{{ item.length }}%</span>
                    </div>
                </div>
            </div>

            <!-- Tools -->
            <div class="flex flex-col gap-1 text-sm w-full">
                <span class="font-medium text-slate-500 dark:text-slate-400 mb-1">Tools</span>
                <div>
                    <div class="flex items-center gap-1 my-2 w-full" v-for="item in tools" :key="item.id">
                        <span class="min-w-24 truncate text-slate-700 dark:text-slate-200">{{ item.name }}</span>
                        <div
                            class="flex-1 h-2 bg-slate-100 dark:bg-slate-700 rounded-full overflow-hidden border border-slate-200 dark:border-slate-600">
                            <div class="h-full rounded-full transition-all duration-500"
                                :style="{ background: item.color, width: item.length + '%' }"></div>
                        </div>
                        <span class="w-8 text-right text-slate-500 dark:text-slate-400">{{ item.length }}%</span>
                    </div>
                </div>
            </div>

        </div>

    </section>
</template>

<style scoped></style>
