<script setup>
import { RouterView } from 'vue-router'
</script>

<template>
  <RouterView />
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Inter', sans-serif;
  line-height: 1.5;
  color: #333;
  overflow-x: hidden;
}

:root {
  --primary-gradient: linear-gradient(90deg, #4776E6 0%, #8E54E9 100%);
  --primary-color: #4776E6;
  --secondary-color: #8E54E9;
  --text-color: #333;
  --text-light: #666;
  --background-light: #f8f9fa;
  --background-white: #ffffff;
  --shadow-sm: 0 5px 15px rgba(0, 0, 0, 0.05);
  --shadow-md: 0 10px 25px rgba(0, 0, 0, 0.1);
  --border-radius-sm: 8px;
  --border-radius-md: 16px;
  --border-radius-lg: 20px;
}
</style>
