<template>
  <div v-if="show" class="h-10 bg-yellow-400 dark:bg-yellow-600 text-white flex items-center gap-3">
    <i class="fa-solid fa-triangle-exclamation ml-6"></i>
    <p>notice</p>
  </div>
  <button @click="setShow">toggle</button>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const show = ref(false)

function setShow() {
  show.value = !show.value
}
</script>
