<script setup>
import { ref, reactive } from 'vue'

const title = ref('Nyan programer')
const info = ref({
  nyans: 100,
  churu: 4
})

let number = ref(5000)
number.value = 3222

function increment() {
  number.value += 1
  bossNyan.age += 1
  bossNyan.bio = 'にゃーーーーん'
  bossNyan.place.parkingArea = 'on the car'
  bossNyan.eat = 'catFood'
}

const bossNyan = reactive({
  name: 'Boss',
  age: 10,
  place: {
    park: 'sandArea',
    parkingArea: 'under the car'
  },
  eat: ref('food')
})
bossNyan.bio = 'nyaaaan'

const count = ref(5)
const count2 = ref(30)
const message = ref('<h1>Nyan</h1>')
const zennDashboard = ref('https://zenn.dev/dashboard')
const zennId = ref('zenn-link')
</script>

<template>
  <h1>Title: {{ title }}</h1>
  <h2>Number: {{ number - 1000 }}</h2>
  <h2>bossNyan age: {{ bossNyan.age }}</h2>
  <h2>bossNyan bio: {{ bossNyan.bio }}</h2>
  <h2>bossNyan parkingArea: {{ bossNyan.place.parkingArea }}</h2>
  <h2>bossNyan eat: {{ bossNyan.eat }}</h2>
  <button @click="increment">ボタン</button>

  <h2>Nyans: {{ info.nyans }}</h2>
  <h3>Churu: {{ info.churu }}</h3>
  <h2>Nyans: {{ info }}</h2>

  <div>{{ 10 + 20 }}</div>
  <div>{{ count + 20 }}</div>
  <div>{{ count + count2 }}</div>
  <div>{{ count > 4 ? 'nyan' : 'nyaaaan' }}</div>

  <div v-html="message"></div>
  <a v-bind:id="zennId" v-bind:href="zennDashboard" target="_blank">Zenn dashboard</a><br>
  <button disabled>Button</button>
</template>

<style>
h1 {
  color: green;
}
h2 {
  color: red;
}
</style>
