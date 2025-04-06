<script setup>
import { ref, computed } from 'vue'

const score = ref(0)
const evaluation = computed(() => {score.value > 3 ? 'Good!!!👍' : 'Bad👎'})
console.log(evaluation);
</script>

<template>
  <p>{{ score > 3 ? 'Good!!!👍' : 'Bad👎' }}</p>
  <p>{{ evaluation }}</p>
  <p>{{ score }}</p>
  <button @click="score++">+1</button>
</template>

<style>
h1 {
  color: green;
}
h2 {
  color: red;
}
</style>
