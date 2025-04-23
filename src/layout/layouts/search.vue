<template>
    <div class="search-bar">
        <input class="rounded-l-xl p-2" placeholder="여기에 검색...">
        <button class="px-1"><i class="fa-solid fa-magnifying-glass"></i></button>
        <button class="px-2 rounded-r-xl"><i class="fa-solid fa-chevron-right"></i></button>
    </div>
</template>

<style>
.search-bar > * {
    background-color: var(--color-neutral-200);
    color: black;
    height: 36px;
}

@media (max-width: 48rem) {
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
        height: 37px;
        border-radius: 0;
    }
    .search-bar button:last-child {
        border-radius: 0;
    }
}
</style>