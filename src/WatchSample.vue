<script setup>
import { ref, watchEffect } from 'vue'

const count = ref(0)
watchEffect(() => {
  console.log('watchEffect')
  console.log(count.value)
})
</script>

<template>
  <p>{{ count }}</p>
  <button @click="count++">+1</button>
</template>

<style>
h1 {
  color: green;
}
h2 {
  color: red;
}
</style>
