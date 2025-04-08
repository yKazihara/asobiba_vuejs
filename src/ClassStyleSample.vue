<script setup>
import { ref } from 'vue'
const isPink = ref(true)
const isBgGreen = ref(true)
const className = ref('pink')
function toggleClass() {
  isPink.value = !isPink.value
  isBgGreen.value = !isBgGreen.value
}
</script>

<template>
  <div class="pink bg-green">Nyan</div>
  <div :class="'pink bg-green'">Nyan</div>
  <div :class="{pink: true, 'bg-green':true}">Nyan</div>
  <div :class="{ pink: true, 'bg-green': false }">Nyan</div>

  <div :class="[className, { 'bg-green': isBgGreen }]">Nyan</div>
  <button @click="toggleClass">Toggle</button>

  <div class="border" :class="[className, { 'bg-green': isBgGreen }]">Nyan</div>
</template>

<style>
.pink {
  color: pink;
}
.bg-green {
  background-color: green;
}
.border {
  border: 2px dotted black;
}
</style>
