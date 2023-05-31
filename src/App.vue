<script setup>
import { defineComponent } from "vue";
import Counter from "./components/Counter.vue";
import EvenNumSum from "./components/EvenNumSum.vue";

defineComponent({
  components: { Counter, EvenNumSum },
});
</script>

<template>
  <Counter></Counter>
  <EvenNumSum></EvenNumSum>
</template>

<style scoped></style>
