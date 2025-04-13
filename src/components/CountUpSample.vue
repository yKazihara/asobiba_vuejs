<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <div><h2>CountUp++</h2></div>
  <p class="red">count:{{ count }}</p>
  <button @click="count++">+1</button>
</template>

<style>

</style>
