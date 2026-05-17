<script setup></script>

<template>
    <section class="flex flex-col border-b border-slate-200 dark:border-slate-700 shadow-xs px-6 lg:px-18 py-6 lg:py-12" id="aboutme">

        <h2 class="text-xl font-medium text-slate-700 dark:text-slate-200">About Me</h2>

        <div class="grid grid-cols-2 gap-4 my-5">

            <!-- Education -->
            <div class="border border-slate-200 dark:border-slate-700 p-4 rounded-2xl">
                <div class="flex flex-col gap-1">
                    <div class="flex items-center gap-1">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                            class="bi bi-mortarboard text-slate-500" viewBox="0 0 16 16">
                            <path
                                d="M8.211 2.047a.5.5 0 0 0-.422 0l-7.5 3.5a.5.5 0 0 0 .025.917l7.5 3a.5.5 0 0 0 .372 0L14 7.14V13a1 1 0 0 0-1 1v2h3v-2a1 1 0 0 0-1-1V6.739l.686-.275a.5.5 0 0 0 .025-.917zM8 8.46 1.758 5.965 8 3.052l6.242 2.913z" />
                            <path
                                d="M4.176 9.032a.5.5 0 0 0-.656.327l-.5 1.7a.5.5 0 0 0 .294.605l4.5 1.8a.5.5 0 0 0 .372 0l4.5-1.8a.5.5 0 0 0 .294-.605l-.5-1.7a.5.5 0 0 0-.656-.327L8 10.466zm-.068 1.873.22-.748 3.496 1.311a.5.5 0 0 0 .352 0l3.496-1.311.22.748L8 12.46z" />
                        </svg>
                        <span class="text-sm text-slate-500">Education</span>
                    </div>

                    <div class="text-sm">
                        <span class="lg:hidden">
                            B.Sc (IT)
                        </span>
                        <span class="hidden lg:inline">
                            Bachelor of Science Program in Information Technology
                        </span>
                        <br>
                        <span>
                            Year 2 · KMUTT
                        </span>
                    </div>
                </div>
            </div>

            <!-- Career goal -->
            <div class="border border-slate-200 dark:border-slate-700 p-4 rounded-2xl">
                <div class="flex flex-col gap-1">
                    <div class="flex items-center gap-1">
                        <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" fill="currentColor"
                            class="bi bi-bullseye text-slate-500" viewBox="0 0 16 16">
                            <path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14m0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16" />
                            <path d="M8 13A5 5 0 1 1 8 3a5 5 0 0 1 0 10m0 1A6 6 0 1 0 8 2a6 6 0 0 0 0 12" />
                            <path d="M8 11a3 3 0 1 1 0-6 3 3 0 0 1 0 6m0 1a4 4 0 1 0 0-8 4 4 0 0 0 0 8" />
                            <path d="M9.5 8a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0" />
                        </svg>
                        <span class="text-sm text-slate-500">Career goal</span>
                    </div>

                    <div class="text-sm">
                        <span>
                            Full-Stack Developer
                        </span>
                    </div>
                </div>
            </div>

            <!-- Interests -->
            <div class="border border-slate-200 dark:border-slate-700 p-4 rounded-2xl">
                <div class="flex flex-col gap-1">
                    <div class="flex items-center gap-1">
                        <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" fill="currentColor"
                            class="bi bi-heart text-slate-500" viewBox="0 0 16 16">
                            <path
                                d="m8 2.748-.717-.737C5.6.281 2.514.878 1.4 3.053c-.523 1.023-.641 2.5.314 4.385.92 1.815 2.834 3.989 6.286 6.357 3.452-2.368 5.365-4.542 6.286-6.357.955-1.886.838-3.362.314-4.385C13.486.878 10.4.28 8.717 2.01zM8 15C-7.333 4.868 3.279-3.04 7.824 1.143q.09.083.176.171a3 3 0 0 1 .176-.17C12.72-3.042 23.333 4.867 8 15" />
                        </svg>
                        <span class="text-sm text-slate-500">Interests</span>
                    </div>

                    <div class="text-sm">
                        <span>
                            Frontend · Backend · Game Developer
                        </span>
                        <br>
                    </div>
                </div>
            </div>

            <!-- Languages -->
            <div class="border border-slate-200 dark:border-slate-700 p-4 rounded-2xl">
                <div class="flex flex-col gap-1">
                    <div class="flex items-center gap-1">
                        <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" fill="currentColor"
                            class="bi bi-translate text-slate-500" viewBox="0 0 16 16">
                            <path
                                d="M4.545 6.714 4.11 8H3l1.862-5h1.284L8 8H6.833l-.435-1.286zm1.634-.736L5.5 3.956h-.049l-.679 2.022z" />
                            <path
                                d="M0 2a2 2 0 0 1 2-2h7a2 2 0 0 1 2 2v3h3a2 2 0 0 1 2 2v7a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2v-3H2a2 2 0 0 1-2-2zm2-1a1 1 0 0 0-1 1v7a1 1 0 0 0 1 1h7a1 1 0 0 0 1-1V2a1 1 0 0 0-1-1zm7.138 9.995q.289.451.63.846c-.748.575-1.673 1.001-2.768 1.292.178.217.451.635.555.867 1.125-.359 2.08-.844 2.886-1.494.777.665 1.739 1.165 2.93 1.472.133-.254.414-.673.629-.89-1.125-.253-2.057-.694-2.82-1.284.681-.747 1.222-1.651 1.621-2.757H14V8h-3v1.047h.765c-.318.844-.74 1.546-1.272 2.13a6 6 0 0 1-.415-.492 2 2 0 0 1-.94.31" />
                        </svg>
                        <span class="text-sm text-slate-500">Education</span>
                    </div>
                    <div class="text-sm">
                        <span>
                            Thai (native) · English (conversational)
                        </span>
                        <br>
                    </div>
                </div>
            </div>

        </div>
    </section>
</template>

<style scoped></style>
