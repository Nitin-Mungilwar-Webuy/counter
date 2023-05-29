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

<template>
  <header>
    <h1>Counter app</h1>
    <p>{{ counter }}</p>
    <button @click="increment">Increment</button>
    <button @click="decrement">Decrement</button>
  </header>

  <main></main>
</template>

<style scoped></style>
