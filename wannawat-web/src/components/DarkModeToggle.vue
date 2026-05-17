<script setup>
import { useDarkMode } from '../composables/useDarkMode';

const { isDark, toggle } = useDarkMode();
</script>

<template>
    <button @click="toggle"
        class="flex items-center gap-2 px-3 py-2.5 w-full text-left rounded-b-xl
               text-slate-700 dark:text-slate-200 hover:text-indigo-500 dark:hover:text-indigo-400
               hover:bg-blue-50 dark:hover:bg-slate-700
               transition-colors duration-200 cursor-pointer"
        :aria-label="isDark ? 'Switch to light mode' : 'Switch to dark mode'">
        <!-- Sun icon (dark mode active → switch to light) -->
        <svg v-if="isDark" xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 shrink-0" fill="none"
            viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <circle cx="12" cy="12" r="5" />
            <path stroke-linecap="round"
                d="M12 2v2M12 20v2M4.22 4.22l1.42 1.42M18.36 18.36l1.42 1.42M2 12h2M20 12h2M4.22 19.78l1.42-1.42M18.36 5.64l1.42-1.42" />
        </svg>
        <!-- Moon icon (light mode active → switch to dark) -->
        <svg v-else xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 shrink-0" fill="none"
            viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round"
                d="M21 12.79A9 9 0 1111.21 3 7 7 0 0021 12.79z" />
        </svg>
        <span class="hidden md:inline">{{ isDark ? 'Light Mode' : 'Dark Mode' }}</span>
    </button>
</template>

<style scoped></style>
