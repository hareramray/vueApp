<template>
  <div>
    <h1>Welcome to Vue 3 + TypeScript!</h1>
    <p>This is a message from TheWelcome component.</p>
  </div>
</template>

<script setup lang="ts">
// You can add TypeScript logic here if needed
import { onMounted, onUpdated } from 'vue';

onMounted(() => {
  console.log("TheWelcome component has been mounted");
});

onUpdated(() => {
  console.log("TheWelcome component re-rendered");
});
</script>

<style scoped>
h1 {
  color: #42b983;
}

</style>