<script setup>
import { ref } from 'vue'
const ok = ref(true)
</script>

<template>
  <button @click="ok = !ok">toggle</button>
  <p v-show="ok">OK!</p>
  <p v-show="!ok">NO!</p>
</template>

<style>

</style>
