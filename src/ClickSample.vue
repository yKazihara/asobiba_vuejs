<script setup>
import { ref, reactive } from 'vue'

const count = ref(0)
function countUp() {
  count.value++
}
</script>

<template>
  <p>{{ count }}</p>
  <button @click="count++">button</button>
  <button @click="countUp">button</button>
</template>

<style>
h1 {
  color: green;
}
h2 {
  color: red;
}
</style>
