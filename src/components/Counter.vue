<template>
  <h1>Counter app</h1>
  <p>{{ counter }}</p>
  <button @click="increment">Increment</button>
  <button @click="decrement">Decrement</button>
</template>
<script setup>
import { ref } from "vue";
const counter = ref(0);
const increment = () => {
  counter.value++;
};
const decrement = () => {
  counter.value--;
};
</script>
<style></style>
