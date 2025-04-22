<template>
    <div class="bg-neutral-100 dark:bg-neutral-900 text-black dark:text-white">
        <!--modern v2-->
        <Header />
        <Banner />
        <main class="m-4 min-h-[100vh]">
            content
        </main>
        <Footer />
    </div>
</template>

<style>
@import "./css/output.css";
@import "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css";
</style>

<script setup lang="ts">
import Header from "./layouts/header.vue";
import Banner from "./layouts/banner.vue";
import Footer from "./layouts/footer.vue";
</script>