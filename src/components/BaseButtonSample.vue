<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <div class="red bg-green" @click="console.log('BaseButton.vue')">
    Click!
    <button>BaseButton</button>
  </div>
</template>

<style>

</style>
