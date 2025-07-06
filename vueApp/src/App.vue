<template>
   
   <div>
      <TheWelcome />
      <Counter />
   </div>
</template>

<script setup lang="ts">

import { ref, onUpdated } from 'vue';
import TheWelcome from './components/TheWelcome.vue';
import Counter from './components/Counter.vue';


onUpdated(() => {
   console.log("Component re-rendered");
});
</script>
