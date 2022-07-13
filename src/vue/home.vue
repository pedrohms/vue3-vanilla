<script setup>
import { ref } from "vue"
let msg = "Hi mom !"
let count = ref(0)
const handleclick = () => {
  console.log("ok")
  console.log(count.value)  
    count.value = count.value + 1
  }
</script>
<template>
  <div>
    <h1>{{ msg }} - {{ count }}</h1>
    <button @click="handleclick">Click me</button>
  </div>
</template>
<style scoped>
  .example {
    color: v-bind("color");
  }
</style>
