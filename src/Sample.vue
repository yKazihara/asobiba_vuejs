<script setup>
import {ref} from "vue";

const title = ref('Nyan programer')
const info = ref({
  nyans: 100,
  churu: 4
})

let number = ref(9999)
console.log(number.value)
console.log(info.value.nyans);
console.log(info.value.churu);

number.value = 2222

function increment() {
  number.value += 1
  console.log(number)
}
</script>

<template>
  <h1>Title: {{ title }}</h1>
  <h2>Number: {{ number - 1000 }}</h2>
  <button @click="increment">ボタン</button>

  <h2>Nyans: {{ info.nyans }}</h2>
  <h3>Churu: {{ info.churu }}</h3>
  <h2>Nyans: {{ info }}</h2>
</template>

<style>
h1 {
  color: green;
}
h2 {
  color: red;
}
</style>
