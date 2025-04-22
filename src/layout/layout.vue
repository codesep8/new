<template>
    <div class="bg-neutral-100 dark:bg-neutral-900">
        <!--modern v2-->
        <Header />
        <Banner />
        <main class="m-4 min-h-[100vh]">
            hid
        </main>
        <Footer />
    </div>
</template>

<style>
@import "./css/output.css";
</style>

<script setup lang="ts">
import Header from "./layouts/header.vue";
import Banner from "./layouts/banner.vue";
import Footer from "./layouts/footer.vue";
</script>