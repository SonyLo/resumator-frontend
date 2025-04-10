<template>
  <div class="feature-card">
    <div class="icon-wrapper">
      <div class="icon" :class="`icon-${icon}`">
        <svg v-if="icon === 'customize'" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M12 4V2M12 22v-2M18 12h2M4 12h2M6.34 6.34L4.93 4.93M19.07 19.07l-1.41-1.41M17.66 6.34l1.41-1.41M6.93 19.07l1.41-1.41M16 12a4 4 0 11-8 0 4 4 0 018 0z" stroke="currentColor" stroke-width="2" stroke-linecap="round" fill="none" />
        </svg>
        <svg v-else-if="icon === 'auto-deploy'" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M12 16l-4-4h2.55v-5h2.9v5H16l-4 4z" fill="currentColor" />
          <path d="M4 20h16a2 2 0 002-2V8a2 2 0 00-2-2H4a2 2 0 00-2 2v10a2 2 0 002 2z" stroke="currentColor" stroke-width="2" fill="none" />
        </svg>
        <svg v-else-if="icon === 'analytics'" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M8 13v5M12 8v10M16 3v15M4 22h16.5" stroke="currentColor" stroke-width="2" stroke-linecap="round" fill="none" />
        </svg>
        <svg v-else-if="icon === 'templates'" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M4 4h16a2 2 0 012 2v12a2 2 0 01-2 2H4a2 2 0 01-2-2V6a2 2 0 012-2z" stroke="currentColor" stroke-width="2" fill="none" />
          <path d="M4 8h16M8 4v16" stroke="currentColor" stroke-width="2" stroke-linecap="round" fill="none" />
        </svg>
      </div>
    </div>
    <h3 class="title">{{ title }}</h3>
    <p class="description">{{ description }}</p>
  </div>
</template>

<script setup>
defineProps({
  icon: {
    type: String,
    required: true
  },
  title: {
    type: String,
    required: true
  },
  description: {
    type: String,
    required: true
  }
});
</script>

<style scoped>
.feature-card {
  background: white;
  border-radius: 16px;
  padding: 30px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
  transition: all 0.3s ease;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  opacity: 0;
  transform: translateY(20px);
}

.feature-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
}

.feature-card.animate-in {
  opacity: 1;
  transform: translateY(0);
}

.icon-wrapper {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  background: linear-gradient(135deg, rgba(71, 118, 230, 0.1) 0%, rgba(142, 84, 233, 0.1) 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 24px;
}

.icon {
  width: 40px;
  height: 40px;
  color: #4776E6;
}

.title {
  font-size: 1.3rem;
  font-weight: 700;
  margin-bottom: 16px;
  color: #333;
}

.description {
  color: #666;
  line-height: 1.6;
}
</style> 