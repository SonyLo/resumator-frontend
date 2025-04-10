<template>
  <div class="testimonial-card">
    <div class="quote-icon">
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M11 7H7a2 2 0 00-2 2v6a2 2 0 002 2h4v6h6v-6a6 6 0 00-6-6V7zm-5 8V9h4v2h-2v4H6zm12 0v-2h-2v-2h4v6h-4v-2h2z" fill="currentColor" />
      </svg>
    </div>
    <div class="testimonial-content">{{ testimonial }}</div>
    <div class="testimonial-footer">
      <div class="avatar">
        <img :src="avatarPath" :alt="name">
      </div>
      <div class="user-info">
        <div class="name">{{ name }}</div>
        <div class="position">{{ position }}</div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { computed } from 'vue';

const props = defineProps({
  name: {
    type: String,
    required: true
  },
  position: {
    type: String,
    required: true
  },
  testimonial: {
    type: String,
    required: true
  },
  avatar: {
    type: String,
    required: true
  }
});

const avatarPath = computed(() => {
  // Динамический импорт SVG файлов
  if (props.avatar === 'avatar1.jpg') return new URL('../assets/avatar1.svg', import.meta.url).href;
  if (props.avatar === 'avatar2.jpg') return new URL('../assets/avatar2.svg', import.meta.url).href;
  if (props.avatar === 'avatar3.jpg') return new URL('../assets/avatar3.svg', import.meta.url).href;
  return new URL('../assets/avatar1.svg', import.meta.url).href; // Значение по умолчанию
});
</script>

<style scoped>
.testimonial-card {
  background: white;
  border-radius: 16px;
  padding: 30px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
  transition: all 0.3s ease;
  min-width: 280px;
  max-width: 350px;
  flex-shrink: 0;
  position: relative;
  opacity: 0;
  transform: translateY(20px);
}

.testimonial-card.animate-in {
  opacity: 1;
  transform: translateY(0);
}

.testimonial-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
}

.quote-icon {
  position: absolute;
  top: 20px;
  right: 20px;
  width: 40px;
  height: 40px;
  color: rgba(71, 118, 230, 0.1);
}

.testimonial-content {
  font-size: 1.1rem;
  line-height: 1.6;
  color: #444;
  margin-bottom: 30px;
  font-style: italic;
}

.testimonial-footer {
  display: flex;
  align-items: center;
}

.avatar {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  overflow: hidden;
  margin-right: 15px;
  flex-shrink: 0;
}

.avatar img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.user-info {
  flex-grow: 1;
}

.name {
  font-weight: 700;
  color: #333;
  margin-bottom: 5px;
}

.position {
  font-size: 0.9rem;
  color: #777;
}
</style> 