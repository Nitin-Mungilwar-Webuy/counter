<template>
  <div class="container">
    <h1>Counter app</h1>
    <p>{{ counter }}</p>
    <button @click="increment">Increment</button>
    <button @click="decrement">Decrement</button>
  </div>
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
<style>
.container {
  width: 400px;
  height: 200px;
  background-color: antiquewhite;
  align-items: center;
}
button {
  padding: 10px;
  background-color: rgb(194, 194, 231);
  margin-right: 10px;
}
p {
  align-items: center;
  margin-left: 100px;
  margin-bottom: 20px;
}
</style>
