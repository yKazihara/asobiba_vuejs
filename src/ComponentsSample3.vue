<script setup>
import { ref } from 'vue'
import ChildComp from '@/components/ChildComponentsSample3.vue'

const msg = ref('from parent')
</script>

<template>
  <ChildComp></ChildComp>
</template>

<style>

</style>
