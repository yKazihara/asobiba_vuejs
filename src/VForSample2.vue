<script setup>
import { ref } from 'vue'
const nyans = ref([
  { id: 1, name: 'kuro' },
  { id: 2, name: 'kuro' },
  { id: 3, name: 'tora' },
  { id: 4, name: 'mike' },
  { id: 5, name: 'tama' }
])
</script>

<template>
  <li v-for="nyan in nyans">{{ nyan }}</li>

  <button @click="nyans.shift()">button</button>
  <li v-for="nyan in nyans" :key="nyan.id"><input type="text" />{{ nyan.name }}</li>
</template>

<style>

</style>
