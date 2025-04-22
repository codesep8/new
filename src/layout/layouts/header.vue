<template>
    <header class="h-15 bg-blue-500 dark:bg-blue-700 text-white font-bold flex items-center">
        <nav class="flex justify-between items-center">
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