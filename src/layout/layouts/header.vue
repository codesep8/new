<template>
    <header class="h-15 bg-blue-500 dark:bg-blue-700 text-white font-bold flex items-center">
        <nav class="flex justify-between items-center w-full">
            <div class="flex items-center gap-6">
                <a href="/" class="ml-6 text-2xl font-bold">theseed</a>
                <a href="/RecentChanges" class="nav-links">
                    <i class="fa-solid fa-clock"></i>
                    최근 변경
                </a>
                <a href="/RecentDiscuss" class="nav-links">
                    <i class="fa-solid fa-comment"></i>
                    최근 토론
                </a>
                <div class="nav-links">
                    <i class="fa-solid fa-toolbox"></i>
                    도구
                </div>
            </div>
            <div class="flex gap-4 items-center">
                <div class="nav-links text-black">
                    <input class="rounded-l-lg bg-neutral-100 h-10 p-2" placeholder="여기에 검색...">
                    <button class="h-10 px-1 bg-neutral-100"><i class="fa-solid fa-magnifying-glass"></i></button>
                    <button class="h-10 px-2 rounded-r-lg bg-neutral-100"><i class="fa-solid fa-chevron-right"></i></button>
                </div>
                <img class="md:mr-6 inline-block size-10 rounded-full" src="https://images.unsplash.com/photo-1568602471122-7832951cc4c5?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=2&w=300&h=300&q=80"/>
                <button class="mr-4 md:hidden rounded text-2xl hover:bg-secondary dark:hover:bg-secondary-dark">
                    <i class="fa-solid fa-bars"></i>
                </button>
            </div>
        </nav>
    </header>
</template>

<style scoped>
@media (max-width: 767px) {
		.nav-links {
				display: none;
		}
}
</style>