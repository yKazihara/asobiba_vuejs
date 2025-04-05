<script setup>
import { ref, reactive } from 'vue'

const count = ref(0)
const count2 = ref(0)
function countUp() {
  count.value++
}
</script>

<template>
  <p>{{ count }}</p>
  <button @click="count++">button</button>
  <button @click="countUp">button</button>

  <p>{{ count2 }}</p>
  <div @click="count2++">
    <button @click.stop="count2 = 50">ボタン</button>
  </div>
</template>

<style>
h1 {
  color: green;
}
h2 {
  color: red;
}
</style>
