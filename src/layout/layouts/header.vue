<template>
    <header class="h-13 bg-blue-500 text-white dark:bg-blue-600 font-bold flex items-center">
        <nav class="flex justify-between items-center w-full">
            <div class="flex items-center gap-3">
                <a href="/" class="ml-6 text-2xl">thetree</a>
                <a href="/RecentChanges" class="nav-links m-3 rounded-xl hover:bg-blue-600">
                    <i class="text-lg fa-solid fa-clock"></i>
                    최근 변경
                </a>
                <a href="/RecentDiscuss" class="nav-links m-3 rounded-xl hover:bg-blue-600">
                    <i class="text-lg fa-solid fa-comment"></i>
                    최근 토론
                </a>
                <div class="nav-links m-3 rounded-xl hover:bg-blue-600">
                    <i class="text-lg fa-solid fa-toolbox"></i>
                    도구
                </div>
            </div>
            <div class="flex gap-4 items-center">
                <Search />
                <img class="md:mr-6 inline-block size-9 rounded-full" src="https://images.unsplash.com/photo-1568602471122-7832951cc4c5?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=2&w=300&h=300&q=80"/>
                <button class="mr-4 md:hidden rounded text-2xl hover:bg-secondary dark:hover:bg-secondary-dark">
                    <i class="fa-solid fa-bars"></i>
                </button>
            </div>
        </nav>
    </header>
</template>

<style>
.nav-links {
    display: flex;
    align-items: center;
    gap: 2px
}

@media (max-width: 48rem) {
    .nav-links {
        display: none;
    }
}
</style>

<script setup lang="ts">
import Search from "./search.vue"
</script>