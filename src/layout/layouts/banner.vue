<template>
    <div v-if="a" class="h-10 bg-yellow-400 dark:bg-yellow-600 text-white flex items-center gap-3">
        <i class="fa-solid fa-triangle-exclamation ml-6"></i>
        <p>notice</p>
    </div>
    <button @click="setA()">a</button>
</template>

<script setup lang="ts">
import { ref } from "vue"

var a = ref(false)

function setA() {
    a != a
}
</script>