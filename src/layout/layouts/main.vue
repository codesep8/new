<template>
    <main class="flex justify-center">
        <div class="flex flex-col md:flex-row gap-4 md:m-4 items-start w-full">
            <div class="bg-white dark:bg-black md:rounded-xl w-full md:w-8/9 min-h-[100vh] p-6 shadow-xl">
                <div class="flex flex-col md:flex-row md:items-center mb-3 justify-between">
                    <div class="flex flex-col">
                        <DocTitle />
                        <p>최근 변경:</p>
                    </div>
                    <h1>content tools</h1>
                </div>
                content
            </div>
            <div class="bg-white dark:bg-black md:rounded-xl w-full md:w-2/9 p-3 shadow-xl">
                <a href="/RecentChanges" class="text-xl font-bold mb-2">
                    <i class="fa-solid fa-clock"></i>
                    최근 변경
                </a>
                <ul>
                    <li>list</li>
                </ul>
            </div>
        </div>
    </main>
</template>

<script setup lang="ts">
import DocTitle from "./title.vue";
</script>