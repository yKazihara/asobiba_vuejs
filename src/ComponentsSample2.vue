<script setup>
import { ref } from 'vue'
import ChildComp from '@/components/ChildComponentsSample2.vue'

const childMsg = ref('No child msg yet')
</script>

<template>
  <ChildComp @response="(msg) => childMsg = msg" />
  <p>{{ childMsg }}</p>
</template>

<style>

</style>
