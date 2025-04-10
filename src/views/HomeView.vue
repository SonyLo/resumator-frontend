<script setup>
</script>

<template>
  <main>
    <div class="home-content">
      <h1>Главная страница</h1>
      <p>Эта страница будет доступна после авторизации</p>
      <router-link to="/">Вернуться на лендинг</router-link>
    </div>
  </main>
</template>

<style scoped>
.home-content {
  text-align: center;
  padding: 50px 20px;
}

h1 {
  margin-bottom: 20px;
  font-size: 2rem;
  font-weight: 700;
}

p {
  margin-bottom: 30px;
  color: #666;
}
</style>
