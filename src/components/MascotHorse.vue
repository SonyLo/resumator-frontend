<template>
  <div class="mascot-horse">
    <img :src="horseImagePath" alt="Маскот лошадка" />
  </div>
</template>

<script setup>
import { ref } from 'vue';

const horseImagePath = ref(new URL('../assets/horse-mascot.svg', import.meta.url).href);
</script>

<style scoped>
.mascot-horse {
  position: absolute;
  bottom: 0;
  right: 0;
  width: 150px;
  height: auto;
  animation: gallop 3s infinite alternate;
}

@keyframes gallop {
  0% {
    transform: translateX(0) scale(1);
  }
  100% {
    transform: translateX(-10px) scale(1.05);
  }
}
</style> 