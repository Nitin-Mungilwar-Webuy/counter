<template>
  <div>
    <p>Computed Property: Even Numbers Sum - {{ evenNumSum }}</p>

    <p>Method Computing: Even Numbers Sum - {{ computeEvenNumbersSum() }}</p>
  </div>
</template>

<script setup>
import { ref, computed } from "vue";
const numArray = ref([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
const evenNumSum = computed(() => {
  return numArray.value.reduce((sum, number) => {
    if (number % 2 === 0) {
      return sum + number;
    }
    return sum;
  }, 0);
});

function computeEvenNumbersSum() {
  return numArray.value.reduce((sum, number) => {
    if (number % 2 === 0) {
      return sum + number;
    }
    return sum;
  }, 0);
}
</script>
<style></style>
