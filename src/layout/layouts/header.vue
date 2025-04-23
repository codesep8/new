<template>
    <header class="h-13 bg-blue-500 text-white dark:bg-blue-600 font-bold flex items-center">
        <nav class="flex justify-between items-center w-full">
            <div class="flex items-center gap-3">
                <a href="/" class="ml-6 text-2xl">theseed</a>
                <a href="/RecentChanges" class="nav-links m-3 rounded-xl hover:bg-blue-600">
                    <i class="text-xl fa-solid fa-clock"></i>
                    최근 변경
                </a>
                <a href="/RecentDiscuss" class="nav-links m-3 rounded-xl hover:bg-blue-600">
                    <i class="text-xl fa-solid fa-comment"></i>
                    최근 토론
                </a>
                <div class="nav-links m-3 rounded-xl hover:bg-blue-600">
                    <i class="text-xl fa-solid fa-toolbox"></i>
                    도구
                </div>
            </div>
            <div class="flex gap-4 items-center">
                <Search />
                <div class="search-bar">
                    <input class="rounded-l-xl p-2" placeholder="여기에 검색...">
                    <button class="px-1"><i class="fa-solid fa-magnifying-glass"></i></button>
                    <button class="px-2 rounded-r-xl"><i class="fa-solid fa-chevron-right"></i></button>
                </div>
                <img class="md:mr-6 inline-block size-9 rounded-full" src="https://images.unsplash.com/photo-1568602471122-7832951cc4c5?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=2&w=300&h=300&q=80"/>
                <button class="mr-4 md:hidden rounded text-2xl hover:bg-secondary dark:hover:bg-secondary-dark">
                    <i class="fa-solid fa-bars"></i>
                </button>
            </div>
        </nav>
    </header>
</template>

<style>
.search-bar > * {
    background-color: var(--color-neutral-200);
    color: black;
    height: 36px;
}

.nav-links {
    display: flex;
    align-items: center;
    gap: 2px
}

@media (max-width: 48rem) {
    .nav-links {
        display: none;
    }
    .search-bar {
        display: flex;
        position: absolute;
        top: 52px;
        left: 0;
        width: 100%;
        z-index: 10;
    }
    .search-bar input {
        height: 37px;
        flex-grow: 1;
        border-radius: 0;
    }
    .search-bar button {
        height: 37px; /* h-10 */
        border-radius: 0; /* Remove rounded corners */
    }
    .search-bar button:last-child {
        border-radius: 0;
    }
}
</style>

<script>
import Search from "./search.vue"
export default {
    components: {
        Search
    }
}
</script>