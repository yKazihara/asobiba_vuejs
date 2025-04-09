<script setup>
import { ref } from 'vue'
const ok = ref(true)
const maybeOk = ref(true)
</script>

<template>
  <button @click="ok = !ok">toggle</button>
  <template v-if="ok">
    <p>OK!</p>
    <p>Hello!</p>
    <p>Nyan!</p>
    <p>Nyan Nyan!</p>
  </template>
</template>

<style>

</style>
