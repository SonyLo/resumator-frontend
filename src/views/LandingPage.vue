<template>
  <div class="landing-page">
    <!-- Hero section -->
    <section class="hero">
      <div class="hero-content">
        <div class="brand-logo">
          <img src="@/assets/logo.svg" alt="Resumator Logo" />
          <h2 class="brand-name">Resumator</h2>
        </div>
        <h1 class="hero-title">
          <span class="gradient-text">Создавайте</span> профессиональное резюме
          <span class="gradient-text">в несколько кликов</span>
        </h1>
        <p class="hero-description">
          Конструктор, который позволяет собрать идеальное резюме с персональным доменом
          и поделиться им с работодателем в один клик
        </p>
        <div class="hero-buttons">
          <button class="button primary">Начать бесплатно</button>
          <a href="#pricing" class="button secondary">Тарифы</a>
        </div>
      </div>
      <div class="hero-image">
        <div class="resume-preview">
          <img :src="resumePreviewPath" alt="Resume Preview" />
          <div class="floating-element fe-1"></div>
          <div class="floating-element fe-2"></div>
        </div>
      </div>
    </section>

    <!-- Infographic section -->
    <!-- <section class="infographic">
      <div class="infographic-content">
        <div class="infographic-center">
          <h2>Infographic Options</h2>
        </div>
        <div class="infographic-items">
          <div class="infographic-item" v-for="n in 6" :key="n">
            <div class="infographic-icon">🔹</div>
            <div class="infographic-text">
              <h3>Lorem Ipsum</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            </div>
          </div>
        </div>
      </div>
    </section> -->

    <!-- Features section -->
    <section class="features">
      <h2 class="section-title">Почему выбирают <span class="gradient-text">Resumator</span></h2>
      
      <div class="features-grid">
        <div class="feature-card">
          <div class="feature-icon">
            <div class="icon-bg"></div>
            <i class="icon-customize"></i>
          </div>
          <h3 class="feature-title">Полная кастомизация</h3>
          <p class="feature-description">Настраивайте блоки, меняйте цвета и шрифты для уникального дизайна</p>
          <div class="feature-hover-effect"></div>
        </div>
        
        <div class="feature-card">
          <div class="feature-icon">
            <div class="icon-bg"></div>
            <i class="icon-auto-deploy"></i>
          </div>
          <h3 class="feature-title">Автоматический деплой</h3>
          <p class="feature-description">Получите персональный домен для вашего резюме автоматически после создания</p>
          <div class="feature-hover-effect"></div>
        </div>
        
        <div class="feature-card">
          <div class="feature-icon">
            <div class="icon-bg"></div>
            <i class="icon-analytics"></i>
          </div>
          <h3 class="feature-title">Аналитика просмотров</h3>
          <p class="feature-description">Узнайте когда и кто просматривал ваше резюме</p>
          <div class="feature-hover-effect"></div>
        </div>
        
        <!-- <div class="feature-card">
          <div class="feature-icon">
            <div class="icon-bg"></div>
            <i class="icon-templates"></i>
          </div>
          <h3 class="feature-title">Готовые шаблоны</h3>
          <p class="feature-description">Выбирайте из десятков профессиональных шаблонов для разных индустрий</p>
          <div class="feature-hover-effect"></div>
        </div> -->
      </div>
    </section>

    <!-- How it works section -->
    <section class="how-it-works">
      <h2 class="section-title">Как это <span class="gradient-text">работает</span></h2>
      
      <div class="steps">
        <div class="step">
          <div class="step-number">1</div>
          <div class="step-content">
            <div class="step-icon">
              <i class="icon-template"></i>
            </div>
            <h3>Выберите шаблон</h3>
            <p>Перетащите понравившийся шаблон в рабочую область одним движением</p>
          </div>
          <div class="step-connector"></div>
        </div>
        
        <div class="step">
          <div class="step-number">2</div>
          <div class="step-content">
            <div class="step-icon">
              <i class="icon-drag"></i>
            </div>
            <h3>Настройте блоки</h3>
            <p>Перетаскивайте блоки в нужном порядке и добавляйте новые по клику</p>
          </div>
          <div class="step-connector"></div>
        </div>
        
        <div class="step">
          <div class="step-number">3</div>
          <div class="step-content">
            <div class="step-icon">
              <i class="icon-customize"></i>
            </div>
            <h3>Персонализируйте</h3>
            <p>Меняйте цвета, шрифты и стили перетаскиванием элементов</p>
          </div>
          <div class="step-connector"></div>
        </div>
        
        <div class="step">
          <div class="step-number">4</div>
          <div class="step-content">
            <div class="step-icon">
              <i class="icon-publish"></i>
            </div>
            <h3>Опубликуйте</h3>
            <p>Получите уникальную ссылку и поделитесь с работодателями</p>
          </div>
        </div>
      </div>
      
      <!-- <div class="drag-preview">
        <div class="drag-element">
          <div class="drag-handle"></div>
          <div class="drag-content">
            <div class="drag-icon">
              <i class="icon-drag"></i>
            </div>
            <div class="drag-text">Перетащите сюда</div>
          </div>
        </div>
      </div> -->
    </section>

    <!-- Testimonials section -->
    <section class="testimonials">
      <h2 class="section-title">Отзывы <span class="gradient-text">пользователей</span></h2>
      
      <div class="testimonial-carousel">
        <div class="carousel-container">
          <div class="carousel-track">
            <div class="testimonial-card">
              <div class="testimonial-avatar">
                <img src="@/assets/avatar1.svg" alt="Андрей К." />
                <div class="avatar-border"></div>
              </div>
              <div class="testimonial-content">
                <div class="testimonial-quote">
                  <i class="icon-quote"></i>
                </div>
                <p class="testimonial-text">Благодаря Resumator я получил работу в своей мечте! Работодатель отметил современный дизайн резюме.</p>
                <div class="testimonial-author">
                  <h4>Андрей К.</h4>
                  <p>Frontend Developer</p>
                </div>
              </div>
            </div>
			
            
            <div class="testimonial-card">
              <div class="testimonial-avatar">
                <img src="@/assets/avatar2.svg" alt="Мария Л." />
                <div class="avatar-border"></div>
              </div>
              <div class="testimonial-content">
                <div class="testimonial-quote">
                  <i class="icon-quote"></i>
                </div>
                <p class="testimonial-text">Очень удобный конструктор. Создала уникальное портфолио с возможностью показать все свои работы.</p>
                <div class="testimonial-author">
                  <h4>Мария Л.</h4>
                  <p>UX/UI Designer</p>
                </div>
              </div>
            </div>
            
            <div class="testimonial-card">
              <div class="testimonial-avatar">
                <img src="@/assets/avatar3.svg" alt="Дмитрий П." />
                <div class="avatar-border"></div>
              </div>
              <div class="testimonial-content">
                <div class="testimonial-quote">
                  <i class="icon-quote"></i>
                </div>
                <p class="testimonial-text">Интуитивно понятный интерфейс и отличные шаблоны. Рекомендую всем, кто ищет работу!</p>
                <div class="testimonial-author">
                  <h4>Дмитрий П.</h4>
                  <p>Product Manager</p>
                </div>
              </div>
            </div>
            
            <div class="testimonial-card">
              <div class="testimonial-avatar">
                <img src="@/assets/avatar1.svg" alt="Елена С." />
                <div class="avatar-border"></div>
              </div>
              <div class="testimonial-content">
                <div class="testimonial-quote">
                  <i class="icon-quote"></i>
                </div>
                <p class="testimonial-text">Создала резюме за 15 минут! Аналитика просмотров помогла понять, кто интересуется моей кандидатурой.</p>
                <div class="testimonial-author">
                  <h4>Елена С.</h4>
                  <p>Marketing Specialist</p>
                </div>
              </div>
            </div>
            
            <div class="testimonial-card">
              <div class="testimonial-avatar">
                <img src="@/assets/avatar2.svg" alt="Игорь М." />
                <div class="avatar-border"></div>
              </div>
              <div class="testimonial-content">
                <div class="testimonial-quote">
                  <i class="icon-quote"></i>
                </div>
                <p class="testimonial-text">Отличный сервис для создания профессионального резюме. Особенно понравилась возможность кастомизации.</p>
                <div class="testimonial-author">
                  <h4>Игорь М.</h4>
                  <p>Backend Developer</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        
        <div class="carousel-controls">
          <button class="carousel-button prev">
            <i class="icon-arrow-left"></i>
          </button>
          <div class="carousel-dots">
            <span class="dot active"></span>
            <span class="dot"></span>
            <span class="dot"></span>
            <span class="dot"></span>
            <span class="dot"></span>
          </div>
          <button class="carousel-button next">
            <i class="icon-arrow-right"></i>
          </button>
        </div>
      </div>
    </section>

    <!-- Pricing section -->
    <section id="pricing" class="pricing">
      <h2 class="section-title">Выберите <span class="gradient-text">тариф</span></h2>
      
      <div class="pricing-cards">
        <div class="pricing-card">
          <div class="card-header">
            <h3>Бесплатный</h3>
            <div class="price">0 ₽</div>
          </div>
          <ul class="features-list">
            <li><i class="icon-check"></i>1 активное резюме</li>
            <li><i class="icon-check"></i>Базовые шаблоны</li>
            <li><i class="icon-check"></i>Поддомен resumator.io</li>
            <li><i class="icon-check"></i>Базовая аналитика</li>
          </ul>
          <button class="button secondary">Начать сейчас</button>
        </div>
        
        <div class="decorative-element"></div>
        
        <div class="pricing-card premium">
          <div class="card-header">
            <h3>Премиум</h3>
            <div class="price">499 ₽<span>/месяц</span></div>
          </div>
          <ul class="features-list">
            <li><i class="icon-check"></i>До 5 активных резюме</li>
            <li><i class="icon-check"></i>Все шаблоны</li>
            <li><i class="icon-check"></i>Собственный домен</li>
            <li><i class="icon-check"></i>Расширенная аналитика</li>
            <li><i class="icon-check"></i>Экспорт в PDF</li>
            <li><i class="icon-check"></i>Приоритетная поддержка</li>
          </ul>
          <button class="button primary">Выбрать тариф</button>
        </div>
      </div>
    </section>

    <!-- Call to action -->
    <section class="cta">
      <div class="">
        <h2 class="cta-title">Готовы создать идеальное резюме?</h2>
        <p class="cta-description">Присоединяйтесь к тысячам пользователей, которые уже нашли работу мечты</p>
        <button class="button primary large ">Создать резюме бесплатно</button>
      </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
      <div class="footer-logo">
        <img src="@/assets/logo.svg" alt="Resumator Logo" />
        <h3>Resumator</h3>
      </div>
      <div class="footer-links">
        <div class="link-group">
          <h4>Продукт</h4>
          <ul>
            <li><a href="#">Возможности</a></li>
            <li><a href="#">Шаблоны</a></li>
            <li><a href="#">Примеры</a></li>
            <li><a href="#">Тарифы</a></li>
          </ul>
        </div>
        <div class="link-group">
          <h4>Компания</h4>
          <ul>
            <li><a href="#">О нас</a></li>
            <li><a href="#">Блог</a></li>
            <li><a href="#">Карьера</a></li>
            <li><a href="#">Контакты</a></li>
          </ul>
        </div>
        <div class="link-group">
          <h4>Поддержка</h4>
          <ul>
            <li><a href="#">Центр помощи</a></li>
            <li><a href="#">FAQ</a></li>
            <li><a href="#">Политика конфиденциальности</a></li>
            <li><a href="#">Условия использования</a></li>
          </ul>
        </div>
      </div>
      <div class="footer-bottom">
        <p>&copy; 2023 Resumator. Все права защищены.</p>
        <div class="social-links">
          <a href="#"><i class="icon-facebook"></i></a>
          <a href="#"><i class="icon-twitter"></i></a>
          <a href="#"><i class="icon-instagram"></i></a>
          <a href="#"><i class="icon-linkedin"></i></a>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
import FeatureCard from '@/components/FeatureCard.vue';
import TestimonialCard from '@/components/TestimonialCard.vue';
import { onMounted, ref } from 'vue';

const resumePreviewPath = ref(new URL('../assets/resume-preview.svg', import.meta.url).href);

onMounted(() => {
  // Initialize animations
  initAnimations();
});

const initAnimations = () => {
  // Add scroll-based animations
  const elements = document.querySelectorAll('.features-grid > *, .step, .pricing-card, .testimonial-slider > *');
  
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('animate-in');
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.1 });
  
  elements.forEach(el => {
    observer.observe(el);
  });
  
  // Add floating animations to elements
  animateFloatingElements();
};

const animateFloatingElements = () => {
  const floatingElements = document.querySelectorAll('.floating-element');
  floatingElements.forEach((el, index) => {
    // Set random initial positions
    const delay = index * 0.5;
    el.style.animationDelay = `${delay}s`;
  });
};
</script>

<style scoped>
.landing-page {
  font-family: 'Inter', sans-serif;
  color: #f8f9fa;
  background-color: #0a0a0a;
  overflow-x: hidden;
}

section {
  padding: 100px 0;
  position: relative;
}

.section-title {
  font-size: 3rem;
  text-align: center;
  margin-bottom: 70px;
  font-weight: 800;
  color: #f8f9fa;
  letter-spacing: -0.02em;
}

.gradient-text {
  background: linear-gradient(135deg, #00F5A0 0%, #00D9F5 100%);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
  font-weight: bold;
}

/* Hero section */
.hero {
  min-height: 100vh;
  display: flex;
  align-items: center;
  background: radial-gradient(circle at top right, #1a1a1a 0%, #0a0a0a 100%);
  position: relative;
  overflow: hidden;
  padding: 60px;
}

.hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('@/assets/grid.svg') repeat;
  opacity: 0.1;
  pointer-events: none;
}

.hero-content {
  flex: 1;
  padding-right: 60px;
  position: relative;
  z-index: 2;
}

.brand-logo {
  display: flex;
  align-items: center;
  margin-bottom: 40px;
}

.brand-logo img {
  height: 48px;
  margin-right: 16px;
  filter: drop-shadow(0 0 10px rgba(0, 245, 160, 0.3));
}

.brand-name {
  font-size: 1.8rem;
  font-weight: 800;
  background: linear-gradient(135deg, #00F5A0 0%, #00D9F5 100%);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
  letter-spacing: -0.02em;
}

.hero-title {
  font-size: 4rem;
  font-weight: 800;
  line-height: 1.1;
  margin-bottom: 30px;
  color: #f8f9fa;
  letter-spacing: -0.03em;
}

.hero-description {
  font-size: 1.4rem;
  line-height: 1.6;
  color: #a0a0a0;
  margin-bottom: 50px;
  max-width: 650px;
}

.hero-buttons {
  display: flex;
  gap: 20px;
}

.button {
  padding: 16px 32px;
  font-size: 1.1rem;
  font-weight: 600;
  border-radius: 12px;
  cursor: pointer;
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  border: none;
  position: relative;
  overflow: hidden;
}

.button.primary {
  background: linear-gradient(135deg, #00F5A0 0%, #00D9F5 100%);
  color: #0a0a0a;
  box-shadow: 0 4px 20px rgba(0, 245, 160, 0.3);
}

.button.secondary {
  background: rgba(255, 255, 255, 0.05);
  color: #00F5A0;
  border: 2px solid rgba(0, 245, 160, 0.3);
  backdrop-filter: blur(10px);
  text-decoration: none;
}

.button.large {
  padding: 20px 40px;
  font-size: 1.2rem;
}

.button.primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 30px rgba(0, 245, 160, 0.4);
}

.button.secondary:hover {
  background: rgba(0, 245, 160, 0.1);
  border-color: #00F5A0;
}

.hero-image {
  flex: 1;
  position: relative;
  z-index: 1;
}

.resume-preview {
  position: relative;
  width: 100%;
  max-width: 650px;
  margin: 0 auto;
}

.resume-preview img {
  width: 100%;
  height: auto;
  border-radius: 24px;
  box-shadow: 0 30px 60px rgba(0, 0, 0, 0.2);
  transform: perspective(1000px) rotateY(-5deg) rotateX(5deg);
  transition: all 0.6s cubic-bezier(0.4, 0, 0.2, 1);
}

.resume-preview:hover img {
  transform: perspective(1000px) rotateY(0deg) rotateX(0deg);
}

/* Floating elements */
.floating-element {
  position: absolute;
  border-radius: 50%;
  background: linear-gradient(135deg, #00F5A0, #00D9F5);
  opacity: 0.15;
  filter: blur(40px);
  animation: float 8s ease-in-out infinite;
}

.fe-1 {
  width: 200px;
  height: 200px;
  top: -50px;
  right: 20%;
}

.fe-2 {
  width: 300px;
  height: 300px;
  bottom: -100px;
  left: 10%;
  background: linear-gradient(135deg, #00D9F5, #00F5A0);
  animation-duration: 10s;
}

@keyframes float {
  0%, 100% {
    transform: translateY(0) scale(1);
  }
  50% {
    transform: translateY(-30px) scale(1.1);
  }
}

/* Features section */
.features {
  background-color: #0f0f0f;
  position: relative;
  padding: 120px 0;
}

.features::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('@/assets/grid.svg') repeat;
  opacity: 0.05;
  pointer-events: none;
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 40px;
  max-width: 1300px;
  margin: 0 auto;
  padding: 0 40px;
}

.feature-card {
  position: relative;
  background: rgba(255, 255, 255, 0.02);
  border-radius: 24px;
  padding: 40px;
  overflow: hidden;
  transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
  border: 1px solid rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(10px);
  z-index: 1;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  height: 100%;
}

.feature-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: radial-gradient(circle at top right, rgba(0, 245, 160, 0.05), transparent 70%);
  opacity: 0;
  transition: opacity 0.5s ease;
  z-index: -1;
}

.feature-card:hover {
  transform: translateY(-10px);
  border-color: rgba(0, 245, 160, 0.2);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
}

.feature-card:hover::before {
  opacity: 1;
}

.feature-card:hover .feature-icon {
  transform: scale(1.1) rotate(5deg);
}

.feature-card:hover .icon-bg {
  transform: scale(1.2);
  opacity: 0.8;
}

.feature-card:hover .feature-hover-effect {
  opacity: 0.1;
  transform: scale(1.5);
}

.feature-icon {
  position: relative;
  width: 70px;
  height: 70px;
  margin-bottom: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: transform 0.5s cubic-bezier(0.4, 0, 0.2, 1);
}

.icon-bg {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 20px;
  background: linear-gradient(135deg, rgba(0, 245, 160, 0.2), rgba(0, 217, 245, 0.2));
  transform: rotate(45deg);
  transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
  z-index: -1;
}

.feature-icon i {
  font-size: 32px;
  color: #00F5A0;
  z-index: 1;
}

.feature-title {
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 16px;
  color: #f8f9fa;
  position: relative;
}

.feature-description {
  font-size: 1.1rem;
  line-height: 1.6;
  color: #a0a0a0;
  margin-bottom: 0;
  flex-grow: 1;
}

.feature-hover-effect {
  position: absolute;
  bottom: -50px;
  right: -50px;
  width: 200px;
  height: 200px;
  border-radius: 50%;
  background: linear-gradient(135deg, #00F5A0, #00D9F5);
  opacity: 0;
  transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
  z-index: -1;
  filter: blur(40px);
}

/* How it works section */
.how-it-works {
  background: linear-gradient(180deg, #0f0f0f 0%, #0a0a0a 100%);
  position: relative;
  padding: 120px 0;
  overflow: hidden;
}

.how-it-works::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('@/assets/grid.svg') repeat;
  opacity: 0.05;
  pointer-events: none;
}

.how-it-works::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 0;
  width: 100%;
  height: 1px;
  background: linear-gradient(90deg, 
    transparent 0%, 
    rgba(0, 245, 160, 0.1) 20%, 
    rgba(0, 217, 245, 0.1) 80%, 
    transparent 100%);
  z-index: 0;
}

.steps {
  display: flex;
  justify-content: space-between;
  max-width: 1300px;
  margin: 0 auto;
  flex-wrap: wrap;
  padding: 0 40px;
  position: relative;
  z-index: 1;
}

.step {
  flex: 1;
  min-width: 250px;
  padding: 40px;
  text-align: center;
  background: rgba(255, 255, 255, 0.02);
  border-radius: 24px;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.05);
  opacity: 0;
  transform: translateY(20px);
  transition: all 0.6s cubic-bezier(0.4, 0, 0.2, 1);
  position: relative;
  margin-bottom: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.step.animate-in {
  opacity: 1;
  transform: translateY(0);
}

.step:hover {
  transform: translateY(-10px);
  background: rgba(255, 255, 255, 0.03);
  border-color: rgba(0, 245, 160, 0.2);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
}

.step:hover .step-number {
  transform: scale(1.1);
  box-shadow: 0 0 30px rgba(0, 245, 160, 0.4);
}

.step:hover .step-icon {
  transform: scale(1.1) rotate(5deg);
}

.step:hover .step-icon i {
  color: #00F5A0;
}

.step-number {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 70px;
  height: 70px;
  border-radius: 50%;
  background: linear-gradient(135deg, #00F5A0 0%, #00D9F5 100%);
  color: #0a0a0a;
  font-size: 1.8rem;
  font-weight: 800;
  margin: 0 auto 30px;
  box-shadow: 0 4px 20px rgba(0, 245, 160, 0.3);
  transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
  position: relative;
  z-index: 2;
}

.step-content {
  position: relative;
  z-index: 2;
}

.step-icon {
  width: 60px;
  height: 60px;
  margin: 0 auto 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: transform 0.5s cubic-bezier(0.4, 0, 0.2, 1);
}

.step-icon i {
  font-size: 28px;
  color: #a0a0a0;
  transition: color 0.5s ease;
}

.step h3 {
  font-size: 1.5rem;
  margin-bottom: 16px;
  color: #f8f9fa;
  font-weight: 700;
}

.step p {
  color: #a0a0a0;
  line-height: 1.6;
  font-size: 1.1rem;
}

.step-connector {
  position: absolute;
  top: 50%;
  right: -30px;
  width: 60px;
  height: 2px;
  background: linear-gradient(90deg, rgba(0, 245, 160, 0.3), rgba(0, 217, 245, 0.3));
  z-index: 1;
}

.step-connector::before {
  content: '';
  position: absolute;
  top: -4px;
  right: 0;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #00F5A0;
  box-shadow: 0 0 10px rgba(0, 245, 160, 0.5);
}

.step:last-child .step-connector {
  display: none;
}

/* Drag preview */
.drag-preview {
  max-width: 1300px;
  margin: 60px auto 0;
  padding: 0 40px;
  position: relative;
  z-index: 1;
  display: flex;
  justify-content: center;
}

.drag-element {
  width: 300px;
  height: 200px;
  background: rgba(255, 255, 255, 0.03);
  border-radius: 16px;
  border: 2px dashed rgba(0, 245, 160, 0.3);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  animation: pulse 2s infinite;
}

.drag-element:hover {
  background: rgba(255, 255, 255, 0.05);
  border-color: rgba(0, 245, 160, 0.5);
  transform: translateY(-5px);
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
}

.drag-handle {
  position: absolute;
  top: 10px;
  left: 10px;
  width: 30px;
  height: 30px;
  background: rgba(0, 245, 160, 0.2);
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.drag-handle::before {
  content: '';
  width: 16px;
  height: 16px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%2300F5A0'%3E%3Cpath d='M10 9h4V6h3l-5-5-5 5h3v3zm-1 1H6V7l-5 5 5 5v-3h3v-4zm14 2l-5-5v3h-3v4h3v3l5-5zm-9 3h-4v3H7l5 5 5-5h-3v-3z'/%3E%3C/svg%3E");
  background-size: contain;
  background-repeat: no-repeat;
}

.drag-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 20px;
}

.drag-icon {
  width: 60px;
  height: 60px;
  background: rgba(0, 245, 160, 0.1);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 15px;
}

.drag-icon i {
  font-size: 28px;
  color: #00F5A0;
}

.drag-text {
  font-size: 1.2rem;
  color: #f8f9fa;
  font-weight: 600;
  text-align: center;
}

@keyframes pulse {
  0% {
    box-shadow: 0 0 0 0 rgba(0, 245, 160, 0.2);
  }
  70% {
    box-shadow: 0 0 0 15px rgba(0, 245, 160, 0);
  }
  100% {
    box-shadow: 0 0 0 0 rgba(0, 245, 160, 0);
  }
}

@media (max-width: 1200px) {
  .steps {
    gap: 30px;
  }
  
  .step {
    min-width: 220px;
  }
  
  .step-connector {
    width: 30px;
    right: -15px;
  }
}

@media (max-width: 1024px) {
  .steps {
    flex-direction: column;
    align-items: center;
    gap: 30px;
  }
  
  .step {
    width: 100%;
    max-width: 500px;
  }
  
  .step-connector {
    display: none;
  }
  
  .step::after {
    content: '';
    position: absolute;
    bottom: -30px;
    left: 50%;
    transform: translateX(-50%);
    width: 2px;
    height: 30px;
    background: linear-gradient(180deg, rgba(0, 245, 160, 0.3), rgba(0, 217, 245, 0.3));
  }
  
  .step:last-child::after {
    display: none;
  }
  
  .drag-element {
    width: 250px;
    height: 180px;
  }
}

@media (max-width: 768px) {
  .step {
    padding: 30px;
  }
  
  .step-number {
    width: 60px;
    height: 60px;
    font-size: 1.5rem;
    margin-bottom: 20px;
  }
  
  .step-icon {
    width: 50px;
    height: 50px;
    margin-bottom: 15px;
  }
  
  .step-icon i {
    font-size: 24px;
  }
  
  .step h3 {
    font-size: 1.3rem;
    margin-bottom: 12px;
  }
  
  .step p {
    font-size: 1rem;
  }
  
  .drag-element {
    width: 220px;
    height: 160px;
  }
  
  .drag-icon {
    width: 50px;
    height: 50px;
    margin-bottom: 10px;
  }
  
  .drag-icon i {
    font-size: 24px;
  }
  
  .drag-text {
    font-size: 1.1rem;
  }
}

/* Pricing section */
.pricing {
  background: linear-gradient(180deg, #0a0a0a 0%, #0f0f0f 100%);
  position: relative;
  padding: 120px 0;
  overflow: hidden;
}

.pricing-cards {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 40px;
  max-width: 1300px;
  margin: 0 auto;
  flex-wrap: wrap;
  padding: 0 40px;
}

.decorative-element {
  width: 2px;
  height: 100px;
  background: linear-gradient(180deg, #00F5A0 0%, #00D9F5 100%);
  border-radius: 1px;
  opacity: 0.5;
}

.pricing-card {
  background: rgba(255, 255, 255, 0.02);
  border-radius: 24px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
  padding: 50px;
  min-width: 300px;
  flex: 1;
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  opacity: 0;
  transform: translateY(20px);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.05);
  position: relative;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.pricing-card.animate-in {
  opacity: 1;
  transform: translateY(0);
}

.pricing-card:hover {
  transform: translateY(-10px);
  background: rgba(255, 255, 255, 0.03);
  border-color: rgba(0, 245, 160, 0.2);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
}

.pricing-card.premium {
  background: linear-gradient(135deg, rgba(0, 245, 160, 0.1) 0%, rgba(0, 217, 245, 0.1) 100%);
  transform: scale(1.05);
  z-index: 2;
  border: 1px solid rgba(0, 245, 160, 0.3);
}

.card-header {
  text-align: center;
  margin-bottom: 40px;
}

.card-header h3 {
  font-size: 1.8rem;
  margin-bottom: 20px;
  color: #f8f9fa;
  font-weight: 700;
}

.price {
  font-size: 3rem;
  font-weight: 800;
  color: #00F5A0;
  letter-spacing: -0.02em;
}

.price span {
  font-size: 1.1rem;
  font-weight: 400;
  color: #a0a0a0;
}

.features-list {
  list-style: none;
  padding: 0;
  margin: 0 0 40px;
}

.features-list li {
  padding: 12px 0;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
  position: relative;
  padding-left: 30px;
  color: #a0a0a0;
}

.features-list li::before {
  content: "✓";
  position: absolute;
  left: 0;
  color: #00F5A0;
  font-weight: bold;
}

.button {
  padding: 16px 32px;
  font-size: 1.1rem;
  font-weight: 600;
  border-radius: 12px;
  cursor: pointer;
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  border: none;
  position: relative;
  overflow: hidden;
}

.button.primary {
  background: linear-gradient(135deg, #00F5A0 0%, #00D9F5 100%);
  color: #0a0a0a;
  box-shadow: 0 4px 20px rgba(0, 245, 160, 0.3);
}

.button.secondary {
  background: rgba(255, 255, 255, 0.05);
  color: #00F5A0;
  border: 2px solid rgba(0, 245, 160, 0.3);
  backdrop-filter: blur(10px);
}

.button.large {
  padding: 20px 40px;
  font-size: 1.2rem;
}

.button.primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 30px rgba(0, 245, 160, 0.4);
}

.button.secondary:hover {
  background: rgba(0, 245, 160, 0.1);
  border-color: #00F5A0;
}

@media (max-width: 1200px) {
  .pricing-card {
    flex: 0 0 calc(50% - 15px);
  }
}

@media (max-width: 768px) {
  .pricing-card {
    flex: 0 0 100%;
    padding: 30px;
  }
  
  .card-header h3 {
    font-size: 1.5rem;
  }
  
  .price {
    font-size: 2.5rem;
  }
  
  .features-list li {
    padding: 10px 0;
  }
  
  .button {
    padding: 14px 28px;
    font-size: 1rem;
  }
}

/* CTA section */
.cta {
  background: linear-gradient(135deg, #e0f7fa 0%, #c8e6c9 100%);
  color: #0a0a0a;
  text-align: center;
  position: relative;
  overflow: hidden;
  padding: 100px 0;
}

.cta::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('@/assets/grid.svg') repeat;
  opacity: 0.05;
  pointer-events: none;
}

.cta-content {
  max-width: 800px;
  margin: 0 auto;
  position: relative;
  z-index: 1;
  background: rgba(255, 255, 255, 0.8);
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
}

.cta-title {
  font-size: 3.5rem;
  margin-bottom: 24px;
  font-weight: 800;
  letter-spacing: -0.02em;
  color: #333;
}

.cta-description {
  font-size: 1.4rem;
  margin-bottom: 50px;
  opacity: 0.9;
  color: #555;
}

.cta-button {
  background: #0a0a0a;
  color: #c8e6c9;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
}

.cta-button:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.2);
  background: #c8e6c9;
  color: #0a0a0a;
}

/* Footer */
.footer {
  background-color: #0a0a0a;
  color: #f8f9fa;
  padding: 80px 40px 40px;
  position: relative;
}

.footer::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('@/assets/grid.svg') repeat;
  opacity: 0.05;
  pointer-events: none;
}

.footer-logo {
  display: flex;
  align-items: center;
  margin-bottom: 50px;
}

.footer-logo img {
  height: 36px;
  margin-right: 12px;
  filter: drop-shadow(0 0 10px rgba(0, 245, 160, 0.3));
}

.footer-links {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin-bottom: 50px;
  position: relative;
  z-index: 1;
}

.link-group {
  min-width: 180px;
  margin-bottom: 30px;
}

.link-group h4 {
  margin-bottom: 20px;
  color: #f8f9fa;
  font-weight: 600;
}

.link-group ul {
  list-style: none;
  padding: 0;
}

.link-group li {
  margin-bottom: 12px;
}

.link-group a {
  color: #a0a0a0;
  text-decoration: none;
  transition: all 0.3s ease;
  font-size: 1.1rem;
}

.link-group a:hover {
  color: #00F5A0;
  transform: translateX(5px);
}

.footer-bottom {
  display: flex;
  justify-content: space-between;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
  padding-top: 40px;
  color: #a0a0a0;
  font-size: 1rem;
  position: relative;
  z-index: 1;
}

.social-links {
  display: flex;
  gap: 20px;
}

.social-links a {
  color: #a0a0a0;
  font-size: 1.4rem;
  transition: all 0.3s ease;
}

.social-links a:hover {
  color: #00F5A0;
  transform: translateY(-3px);
}

/* Responsive styles */
@media (max-width: 1200px) {
  .hero-title {
    font-size: 3.5rem;
  }
  
  .section-title {
    font-size: 2.5rem;
  }
}

@media (max-width: 1024px) {
  .hero {
    flex-direction: column;
    padding: 80px 40px;
  }
  
  .hero-content {
    padding-right: 0;
    margin-bottom: 80px;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .hero-title {
    font-size: 3rem;
  }
  
  .section-title {
    font-size: 2.2rem;
  }
  
  .steps {
    flex-direction: column;
    align-items: center;
    gap: 30px;
  }
  
  .pricing-card.premium {
    transform: scale(1);
  }
}

@media (max-width: 768px) {
  .hero-title {
    font-size: 2.5rem;
  }
  
  .hero-description {
    font-size: 1.2rem;
  }
  
  .section-title {
    font-size: 2rem;
    margin-bottom: 50px;
  }
  
  .pricing-cards {
    flex-direction: column;
    align-items: center;
  }
  
  .pricing-card {
    width: 100%;
    max-width: 450px;
  }
  
  .footer-links {
    flex-direction: column;
  }
  
  .footer-bottom {
    flex-direction: column;
    align-items: center;
    gap: 30px;
    text-align: center;
  }
  
  .features-grid {
    grid-template-columns: 1fr;
    gap: 30px;
  }
  
  .feature-card {
    padding: 30px;
  }
  
  .feature-icon {
    width: 60px;
    height: 60px;
    margin-bottom: 20px;
  }
  
  .feature-icon i {
    font-size: 28px;
  }
  
  .feature-title {
    font-size: 1.3rem;
  }
  
  .feature-description {
    font-size: 1rem;
  }
}

/* Testimonials section */
.testimonials {
  background: linear-gradient(180deg, #0a0a0a 0%, #0f0f0f 100%);
  position: relative;
  padding: 120px 0;
  overflow: hidden;
}

.testimonials::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('@/assets/grid.svg') repeat;
  opacity: 0.05;
  pointer-events: none;
}

.testimonial-carousel {
  max-width: 1300px;
  margin: 0 auto;
  padding: 0 40px;
  position: relative;
  z-index: 1;
}

.carousel-container {
  position: relative;
  overflow: hidden;
  margin-bottom: 40px;
}

.carousel-track {
  display: flex;
  transition: transform 0.6s cubic-bezier(0.4, 0, 0.2, 1);
  gap: 30px;
}

.testimonial-card {
  flex: 0 0 calc(33.333% - 20px);
  background: rgba(255, 255, 255, 0.02);
  border-radius: 24px;
  padding: 40px;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.05);
  transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
  position: relative;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  min-width: 300px;
}

.testimonial-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: radial-gradient(circle at top right, rgba(0, 245, 160, 0.05), transparent 70%);
  opacity: 0;
  transition: opacity 0.5s ease;
  z-index: -1;
}

.testimonial-card:hover {
  transform: translateY(-10px);
  border-color: rgba(0, 245, 160, 0.2);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
}

.testimonial-card:hover::before {
  opacity: 1;
}

.testimonial-avatar {
  position: relative;
  width: 100px;
  height: 100px;
  margin-bottom: 30px;
}

.testimonial-avatar img {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  object-fit: cover;
  position: relative;
  z-index: 2;
}

.avatar-border {
  position: absolute;
  top: -5px;
  left: -5px;
  right: -5px;
  bottom: -5px;
  border-radius: 50%;
  background: linear-gradient(135deg, #00F5A0 0%, #00D9F5 100%);
  z-index: 1;
  opacity: 0.5;
  animation: rotate 10s linear infinite;
}

@keyframes rotate {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

.testimonial-content {
  position: relative;
  z-index: 2;
}

.testimonial-quote {
  margin-bottom: 20px;
}

.testimonial-quote i {
  font-size: 24px;
  color: #00F5A0;
  opacity: 0.7;
}

.testimonial-text {
  font-size: 1.1rem;
  line-height: 1.6;
  color: #f8f9fa;
  margin-bottom: 30px;
  position: relative;
}

.testimonial-text::before {
  content: '"';
  position: absolute;
  top: -20px;
  left: -10px;
  font-size: 60px;
  color: rgba(0, 245, 160, 0.1);
  font-family: serif;
  line-height: 1;
}

.testimonial-text::after {
  content: '"';
  position: absolute;
  bottom: -40px;
  right: -10px;
  font-size: 60px;
  color: rgba(0, 245, 160, 0.1);
  font-family: serif;
  line-height: 1;
}

.testimonial-author {
  margin-top: auto;
}

.testimonial-author h4 {
  font-size: 1.2rem;
  font-weight: 700;
  color: #f8f9fa;
  margin-bottom: 5px;
}

.testimonial-author p {
  font-size: 1rem;
  color: #00F5A0;
  font-weight: 500;
}

.carousel-controls {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
}

.carousel-button {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.1);
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 0.3s ease;
}

.carousel-button i {
  font-size: 20px;
  color: #f8f9fa;
  transition: all 0.3s ease;
}

.carousel-button:hover {
  background: rgba(0, 245, 160, 0.1);
  border-color: rgba(0, 245, 160, 0.3);
  transform: scale(1.1);
}

.carousel-button:hover i {
  color: #00F5A0;
}

.carousel-dots {
  display: flex;
  gap: 10px;
}

.dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.2);
  cursor: pointer;
  transition: all 0.3s ease;
}

.dot.active {
  background: #00F5A0;
  transform: scale(1.3);
}

@media (max-width: 1200px) {
  .testimonial-card {
    flex: 0 0 calc(50% - 15px);
  }
}

@media (max-width: 768px) {
  .testimonial-card {
    flex: 0 0 100%;
    padding: 30px;
  }
  
  .testimonial-avatar {
    width: 80px;
    height: 80px;
    margin-bottom: 20px;
  }
  
  .testimonial-text {
    font-size: 1rem;
    margin-bottom: 20px;
  }
  
  .testimonial-author h4 {
    font-size: 1.1rem;
  }
  
  .testimonial-author p {
    font-size: 0.9rem;
  }
  
  .carousel-button {
    width: 40px;
    height: 40px;
  }
  
  .carousel-button i {
    font-size: 16px;
  }
}

html {
  scroll-behavior: smooth;
}
</style> 