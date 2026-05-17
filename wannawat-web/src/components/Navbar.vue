<script setup>
import { ref } from 'vue';
import ProfileDropdown from './ProfileDropdown.vue';
import DarkModeToggle from './DarkModeToggle.vue';

const isMenuOpen = ref(false);

function toggleMenu() {
    isMenuOpen.value = !isMenuOpen.value;
}
</script>

<template>
    <nav class="relative px-6 border-b border-slate-200 dark:border-slate-700 shadow-xs md:px-8 py-4">
        <!-- Top bar -->
        <div class="flex justify-between items-center">
            <!-- Brand -->
            <span
                class="flex justify-start items-center gap-3 text-lg text-blue-500 font-bold md:px-6 py-2 rounded-4xl md:text-2xl">
                Wannawat
            </span>

            <!-- Desktop Nav Links -->
            <div class="hidden lg:flex justify-center items-center gap-14 border shadow-lg px-8 py-4 rounded-4xl transition-colors duration-300
                       border-slate-200 bg-white/80 dark:border-slate-700 dark:bg-slate-800/80 backdrop-blur-sm">
                <a href="#"
                    class="text-slate-700 hover:text-indigo-500 transition-colors dark:text-white dark:hover:text-blue-400">Home</a>
                <a href="#aboutme"
                    class="text-slate-700 hover:text-indigo-500 transition-colors dark:text-white dark:hover:text-blue-400">About
                    me</a>
                <a href="#skills"
                    class="text-slate-700 hover:text-indigo-500 transition-colors dark:text-white dark:hover:text-blue-400">Skills</a>
                <a href="#projects"
                    class="text-slate-700 hover:text-indigo-500 transition-colors dark:text-white dark:hover:text-blue-400">Projects</a>
                <a href="#contact"
                    class="text-slate-700 hover:text-indigo-500 transition-colors dark:text-white dark:hover:text-blue-400">Contacts</a>
            </div>

            <!-- Right side: hamburger (mobile) + profile -->
            <div class="flex items-center gap-3">
                <!-- Hamburger Button (mobile only) -->
                <button @click="toggleMenu" class="lg:hidden flex flex-col justify-center items-center w-10 h-10 rounded-xl dark:text-white
                           border border-slate-200 dark:border-slate-700
                           bg-white/80 dark:bg-slate-800/80 backdrop-blur-sm shadow-sm
                           hover:bg-slate-50 dark:hover:bg-slate-700 transition-colors duration-200"
                    aria-label="Toggle menu">
                    <span class="hamburger-line" :class="{ 'rotate-45 translate-y-[7px]': isMenuOpen }"></span>
                    <span class="hamburger-line" :class="{ 'opacity-0': isMenuOpen }"></span>
                    <span class="hamburger-line" :class="{ '-rotate-45 translate-y-[-7px]': isMenuOpen }"></span>
                </button>

                <ProfileDropdown />
            </div>
        </div>

        <!-- Mobile Menu -->
        <div class="lg:hidden absolute left-0 right-0 px-6 md:px-8 z-50" style="top: 100%">
        <Transition name="mobile-menu">
            <div v-if="isMenuOpen" class="flex flex-col gap-1 border border-slate-200 dark:border-slate-700
                       bg-white/90 dark:bg-slate-800/90 backdrop-blur-sm rounded-2xl shadow-lg px-4 py-3">
                <div class="flex justify-between items-center gap-3 px-1 py-1 mb-1">
                    <div class="flex items-center gap-5">
                        <img src="../../public/wannawat-circle-removebg.png" alt="Wannawat Pic" class="rounded-full size-10">
                        <span class="font-medium text-slate-700 dark:text-white">Wannawat</span>    
                    </div>
                    <div class="border border-slate-700 rounded-full w-fit h-fit">
                        <DarkModeToggle />
                    </div>
                </div>

                <a href="#" @click="isMenuOpen = false" class="mobile-nav-link">Home</a>
                <a href="#aboutme" @click="isMenuOpen = false" class="mobile-nav-link">About me</a>
                <a href="#skills" @click="isMenuOpen = false" class="mobile-nav-link">Skills</a>
                <a href="#projects" @click="isMenuOpen = false" class="mobile-nav-link">Projects</a>
                <a href="#contact" @click="isMenuOpen = false" class="mobile-nav-link">Contacts</a>
            </div>
        </Transition>
        </div>
    </nav>
</template>

<style scoped>
.hamburger-line {
    display: block;
    width: 20px;
    height: 2px;
    margin: 2.5px 0;
    background-color: currentColor;
    border-radius: 2px;
    transition: transform 0.25s ease, opacity 0.25s ease;
    /* slate-700 */
}

:global(.dark) .hamburger-line {
    color: white;
    /* slate-200 */
}

.mobile-nav-link {
    display: block;
    padding: 10px 12px;
    font-size: 0.95rem;
    transition: background-color 0.2s ease, color 0.2s ease;
    /* slate-700 */
}

.mobile-nav-link:hover {
    background-color: rgb(239 246 255);
    /* blue-50 */
    color: rgb(59 130 246);
    /* blue-500 */
}

:global(.dark) .mobile-nav-link {
    color: white;
    /* slate-200 */
}

:global(.dark) .mobile-nav-link:hover {
    background-color: rgb(51 65 85);
    /* slate-700 */
    color: rgb(96 165 250);
    /* blue-400 */
}

/* Mobile menu slide-down animation */
.mobile-menu-enter-active,
.mobile-menu-leave-active {
    transition: opacity 0.25s ease, transform 0.25s ease;
}

.mobile-menu-enter-from,
.mobile-menu-leave-to {
    opacity: 0;
    transform: translateY(-8px);
}
</style>
