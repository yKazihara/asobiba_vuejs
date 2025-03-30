<script setup>
const title = 'Nyan programer'
let number = 9999
function increment() {
  console.log('クリック！');
}
</script>

<template>
  <h1>Title: {{ title }}</h1>
  <h2>Number: {{ number - 1000 }}</h2>
  <button @click="increment">ボタン</button>
</template>

<style>
h1 {
  color: green;
}
h2 {
  color: red;
}
</style>
