<template>
  <div>
    <h1>Counter: {{ count }}</h1>
    <button @click="increment">Increment</button>
    <button @click="decrement">Decrement</button>
  </div>
</template>

<script setup lang="ts">
import { ref, onUpdated, onMounted } from 'vue';

onMounted(() => {
  console.log("Counter Component has been mounted");
});

const count = ref<number>(0);

const increment = () => {
  count.value++;
};

const decrement = () => {
  count.value--;
};

onUpdated(() => {
  console.log("Counter Component re-rendered");
});
</script>

<style scoped>
button {
  margin: 0 5px;
}
</style>