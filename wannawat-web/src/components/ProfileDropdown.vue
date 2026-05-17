<script setup>
import { ref } from 'vue'
import DarkModeToggle from './DarkModeToggle.vue'

const isOpen = ref(false);

</script>

<template>
    <div class="hidden lg:inline-block relative">
        <button @click="isOpen = !isOpen"
            class="flex justify-center items-center border border-slate-200 dark:border-slate-700 shadow-md gap-3 px-3 py-2 rounded-4xl cursor-pointer"
            :class="isOpen ? 'round-t-2xl rounded-b-none border-b-transparent shadow-none' : 'rounded2xl shadow-md'"
            id="dropdownButton">
            <img src="../../public/wannawat-square.jpeg" alt="Wannawat Pic" class="rounded-full size-10">
            <span class="hidden md:inline">Wannawat</span>
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                class="bi bi-caret-down-fill" viewBox="0 0 16 16" :class="isOpen ? 'rotate-180' : 'rotate-0'">
                <path
                    d="M7.247 11.14 2.451 5.658C1.885 5.013 2.345 4 3.204 4h9.592a1 1 0 0 1 .753 1.659l-4.796 5.48a1 1 0 0 1-1.506 0z" />
            </svg>
        </button>

        <!-- Dropdown menu -->
        <div class="flex flex-col absolute z-10 w-full border-x rounded-b-2xl bg-white dark:border-slate-700 dark:bg-slate-800 border-slate-200 shadow-md"
            :class="{ 'hidden': !isOpen }" id="dropdownMenu">

            <!-- Dark Mode Toggle -->
            <div class="border-t border-slate-300 dark:border-slate-700">
                <DarkModeToggle class="rounded-none"/>
            </div>

            <!-- <a href=""
                class="border-t border-slate-300 dark:border-slate-700 px-3 py-2 text-slate-700 dark:text-slate-200 hover:text-blue-500">โปรไฟล์</a>
            <a href=""
                class="border-t border-slate-300 dark:border-slate-700 px-3 py-2 text-slate-700 dark:text-slate-200 hover:text-blue-500">ตั้งค่า</a>
            <a href=""
                class="border-t border-slate-300 dark:border-slate-700 px-3 py-2 text-red-500 hover:text-red-700">ออกจากระบบ</a> -->
        </div>

    </div>
</template>

<style scoped></style>