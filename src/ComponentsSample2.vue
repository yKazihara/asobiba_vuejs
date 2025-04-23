<script setup>
import { ref } from 'vue'
import ChildComp from '@/components/ChildComponentsSample2.vue'

const greeting = ref('Hello from parent')
</script>

<template>
  <ChildComp :msg="greeting" />
</template>

<style>

</style>
