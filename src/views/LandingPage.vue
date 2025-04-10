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
          <button class="button secondary">Примеры работ</button>
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

    <!-- Features section -->
    <section class="features">
      <h2 class="section-title">Почему выбирают <span class="gradient-text">Resumator</span></h2>
      
      <div class="features-grid">
        <feature-card 
          icon="customize" 
          title="Полная кастомизация" 
          description="Настраивайте блоки, меняйте цвета и шрифты для уникального дизайна"
        />
        <feature-card 
          icon="auto-deploy" 
          title="Автоматический деплой" 
          description="Получите персональный домен для вашего резюме автоматически после создания"
        />
        <feature-card 
          icon="analytics" 
          title="Аналитика просмотров" 
          description="Узнайте когда и кто просматривал ваше резюме"
        />
        <feature-card 
          icon="templates" 
          title="Готовые шаблоны" 
          description="Выбирайте из десятков профессиональных шаблонов для разных индустрий"
        />
      </div>
    </section>

    <!-- How it works section -->
    <section class="how-it-works">
      <h2 class="section-title">Как это <span class="gradient-text">работает</span></h2>
      
      <div class="steps">
        <div class="step">
          <div class="step-number">1</div>
          <h3>Выберите шаблон</h3>
          <p>Просмотрите галерею профессиональных шаблонов и выберите подходящий</p>
        </div>
        <div class="step">
          <div class="step-number">2</div>
          <h3>Заполните информацию</h3>
          <p>Добавьте свой опыт, навыки и образование в удобном редакторе</p>
        </div>
        <div class="step">
          <div class="step-number">3</div>
          <h3>Настройте дизайн</h3>
          <p>Персонализируйте цвета, шрифты и расположение блоков</p>
        </div>
        <div class="step">
          <div class="step-number">4</div>
          <h3>Опубликуйте резюме</h3>
          <p>Получите уникальную ссылку и поделитесь с работодателями</p>
        </div>
      </div>
    </section>

    <!-- Testimonials section -->
    <section class="testimonials">
      <h2 class="section-title">Отзывы <span class="gradient-text">пользователей</span></h2>
      
      <div class="testimonial-slider">
        <testimonial-card 
          name="Андрей К." 
          position="Frontend Developer" 
          testimonial="Благодаря Resumator я получил работу в своей мечте! Работодатель отметил современный дизайн резюме."
          avatar="avatar1.jpg"
        />
        <testimonial-card 
          name="Мария Л." 
          position="UX/UI Designer" 
          testimonial="Очень удобный конструктор. Создала уникальное портфолио с возможностью показать все свои работы."
          avatar="avatar2.jpg"
        />
        <testimonial-card 
          name="Дмитрий П." 
          position="Product Manager" 
          testimonial="Интуитивно понятный интерфейс и отличные шаблоны. Рекомендую всем, кто ищет работу!"
          avatar="avatar3.jpg"
        />
      </div>
    </section>

    <!-- Pricing section -->
    <section class="pricing">
      <h2 class="section-title">Выберите <span class="gradient-text">тариф</span></h2>
      
      <div class="pricing-cards">
        <div class="pricing-card">
          <div class="card-header">
            <h3>Бесплатный</h3>
            <div class="price">0 ₽</div>
          </div>
          <ul class="features-list">
            <li>1 активное резюме</li>
            <li>Базовые шаблоны</li>
            <li>Поддомен resumator.io</li>
            <li>Базовая аналитика</li>
          </ul>
          <button class="button secondary">Начать сейчас</button>
        </div>
        
        <div class="pricing-card premium">
          <div class="card-header">
            <h3>Премиум</h3>
            <div class="price">499 ₽<span>/месяц</span></div>
          </div>
          <ul class="features-list">
            <li>До 5 активных резюме</li>
            <li>Все шаблоны</li>
            <li>Собственный домен</li>
            <li>Расширенная аналитика</li>
            <li>Экспорт в PDF</li>
            <li>Приоритетная поддержка</li>
          </ul>
          <button class="button primary">Выбрать тариф</button>
        </div>
        
        <div class="pricing-card">
          <div class="card-header">
            <h3>Корпоративный</h3>
            <div class="price">По запросу</div>
          </div>
          <ul class="features-list">
            <li>Неограниченное количество резюме</li>
            <li>Все функции Премиума</li>
            <li>Брендирование</li>
            <li>API-интеграция</li>
            <li>Персональный менеджер</li>
          </ul>
          <button class="button secondary">Запросить демо</button>
        </div>
      </div>
    </section>

    <!-- Call to action -->
    <section class="cta">
      <div class="cta-content">
        <h2>Готовы создать идеальное резюме?</h2>
        <p>Присоединяйтесь к тысячам пользователей, которые уже нашли работу мечты</p>
        <button class="button primary large">Создать резюме бесплатно</button>
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
  color: #333;
  overflow-x: hidden;
}

section {
  padding: 80px 0;
  position: relative;
}

.section-title {
  font-size: 2.5rem;
  text-align: center;
  margin-bottom: 60px;
  font-weight: 700;
}

.gradient-text {
  background: linear-gradient(90deg, #4776E6 0%, #8E54E9 100%);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
  font-weight: bold;
}

/* Hero section */
.hero {
  min-height: 90vh;
  display: flex;
  align-items: center;
  background: linear-gradient(180deg, #f8f9fa 0%, #ffffff 100%);
  position: relative;
  overflow: hidden;
  padding: 40px;
}

.hero-content {
  flex: 1;
  padding-right: 40px;
  position: relative;
  z-index: 2;
}

.brand-logo {
  display: flex;
  align-items: center;
  margin-bottom: 30px;
}

.brand-logo img {
  height: 40px;
  margin-right: 12px;
}

.brand-name {
  font-size: 1.5rem;
  font-weight: 700;
  background: linear-gradient(90deg, #4776E6 0%, #8E54E9 100%);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
}

.hero-title {
  font-size: 3.5rem;
  font-weight: 800;
  line-height: 1.2;
  margin-bottom: 24px;
}

.hero-description {
  font-size: 1.25rem;
  line-height: 1.6;
  color: #555;
  margin-bottom: 40px;
  max-width: 600px;
}

.hero-buttons {
  display: flex;
  gap: 16px;
}

.button {
  padding: 12px 28px;
  font-size: 1rem;
  font-weight: 600;
  border-radius: 8px;
  cursor: pointer;
  transition: all 0.3s ease;
  border: none;
}

.button.primary {
  background: linear-gradient(90deg, #4776E6 0%, #8E54E9 100%);
  color: white;
  box-shadow: 0 4px 12px rgba(71, 118, 230, 0.3);
}

.button.secondary {
  background: white;
  color: #4776E6;
  border: 2px solid #4776E6;
}

.button.large {
  padding: 16px 32px;
  font-size: 1.1rem;
}

.button.primary:hover {
  box-shadow: 0 6px 16px rgba(71, 118, 230, 0.4);
  transform: translateY(-2px);
}

.button.secondary:hover {
  background: rgba(71, 118, 230, 0.1);
}

.hero-image {
  flex: 1;
  position: relative;
  z-index: 1;
}

.resume-preview {
  position: relative;
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
}

.resume-preview img {
  width: 100%;
  height: auto;
  border-radius: 16px;
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  transform: perspective(1000px) rotateY(-5deg) rotateX(5deg);
  transition: all 0.5s ease;
}

.resume-preview:hover img {
  transform: perspective(1000px) rotateY(0deg) rotateX(0deg);
}

/* Floating elements */
.floating-element {
  position: absolute;
  border-radius: 50%;
  background: linear-gradient(45deg, #4776E6, #8E54E9);
  opacity: 0.8;
  filter: blur(20px);
  animation: float 6s ease-in-out infinite;
}

.fe-1 {
  width: 100px;
  height: 100px;
  top: -30px;
  right: 20%;
}

.fe-2 {
  width: 150px;
  height: 150px;
  bottom: -50px;
  left: 10%;
  background: linear-gradient(45deg, #FF8E53, #FE6B8B);
  animation-duration: 8s;
}

@keyframes float {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-20px);
  }
}

/* Features section */
.features {
  background-color: #ffffff;
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 30px;
  max-width: 1200px;
  margin: 0 auto;
}

/* How it works section */
.how-it-works {
  background-color: #f8f9fa;
}

.steps {
  display: flex;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  flex-wrap: wrap;
}

.step {
  flex: 1;
  min-width: 200px;
  padding: 30px;
  text-align: center;
  opacity: 0;
  transform: translateY(20px);
  transition: all 0.6s ease;
}

.step.animate-in {
  opacity: 1;
  transform: translateY(0);
}

.step-number {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background: linear-gradient(90deg, #4776E6 0%, #8E54E9 100%);
  color: white;
  font-size: 1.5rem;
  font-weight: 700;
  margin: 0 auto 20px;
}

.step h3 {
  font-size: 1.3rem;
  margin-bottom: 12px;
}

.step p {
  color: #666;
}

/* Testimonials section */
.testimonials {
  background-color: white;
}

.testimonial-slider {
  display: flex;
  gap: 30px;
  max-width: 1200px;
  margin: 0 auto;
  overflow-x: auto;
  padding: 20px 0;
  -ms-overflow-style: none;
  scrollbar-width: none;
}

.testimonial-slider::-webkit-scrollbar {
  display: none;
}

/* Pricing section */
.pricing {
  background-color: #f8f9fa;
}

.pricing-cards {
  display: flex;
  justify-content: center;
  gap: 30px;
  max-width: 1200px;
  margin: 0 auto;
  flex-wrap: wrap;
}

.pricing-card {
  background: white;
  border-radius: 16px;
  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.05);
  padding: 40px;
  min-width: 280px;
  flex: 1;
  transition: all 0.3s ease;
  opacity: 0;
  transform: translateY(20px);
}

.pricing-card.animate-in {
  opacity: 1;
  transform: translateY(0);
}

.pricing-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
}

.pricing-card.premium {
  background: linear-gradient(135deg, #F5F7FA 0%, #E3E6E9 100%);
  transform: scale(1.05);
  z-index: 2;
}

.card-header {
  text-align: center;
  margin-bottom: 30px;
}

.card-header h3 {
  font-size: 1.5rem;
  margin-bottom: 16px;
}

.price {
  font-size: 2.5rem;
  font-weight: 700;
  color: #4776E6;
}

.price span {
  font-size: 1rem;
  font-weight: 400;
  color: #777;
}

.features-list {
  list-style: none;
  padding: 0;
  margin: 0 0 30px;
}

.features-list li {
  padding: 10px 0;
  border-bottom: 1px solid #eee;
  position: relative;
  padding-left: 25px;
}

.features-list li::before {
  content: "✓";
  position: absolute;
  left: 0;
  color: #4776E6;
  font-weight: bold;
}

/* CTA section */
.cta {
  background: linear-gradient(90deg, #4776E6 0%, #8E54E9 100%);
  color: white;
  text-align: center;
}

.cta-content {
  max-width: 700px;
  margin: 0 auto;
}

.cta h2 {
  font-size: 2.5rem;
  margin-bottom: 20px;
}

.cta p {
  font-size: 1.2rem;
  margin-bottom: 40px;
  opacity: 0.9;
}

.cta .button.primary {
  background: white;
  color: #4776E6;
}

/* Footer */
.footer {
  background-color: #282c34;
  color: white;
  padding: 60px 40px 30px;
}

.footer-logo {
  display: flex;
  align-items: center;
  margin-bottom: 40px;
}

.footer-logo img {
  height: 30px;
  margin-right: 10px;
}

.footer-links {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin-bottom: 40px;
}

.link-group {
  min-width: 160px;
  margin-bottom: 20px;
}

.link-group h4 {
  margin-bottom: 16px;
  color: #ddd;
}

.link-group ul {
  list-style: none;
  padding: 0;
}

.link-group li {
  margin-bottom: 8px;
}

.link-group a {
  color: #aaa;
  text-decoration: none;
  transition: color 0.2s;
}

.link-group a:hover {
  color: #4776E6;
}

.footer-bottom {
  display: flex;
  justify-content: space-between;
  border-top: 1px solid #444;
  padding-top: 30px;
  color: #aaa;
  font-size: 0.9rem;
}

.social-links {
  display: flex;
  gap: 15px;
}

.social-links a {
  color: #aaa;
  font-size: 1.2rem;
  transition: color 0.2s;
}

.social-links a:hover {
  color: #4776E6;
}

/* Animations */
@keyframes animateIn {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.animate-in {
  animation: animateIn 0.6s forwards;
}

/* Responsive styles */
@media (max-width: 1024px) {
  .hero {
    flex-direction: column;
    padding: 60px 20px;
  }
  
  .hero-content {
    padding-right: 0;
    margin-bottom: 60px;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .hero-title {
    font-size: 2.8rem;
  }
  
  .section-title {
    font-size: 2rem;
  }
  
  .steps {
    flex-direction: column;
    align-items: center;
  }
  
  .pricing-card.premium {
    transform: scale(1);
  }
}

@media (max-width: 768px) {
  .hero-title {
    font-size: 2.2rem;
  }
  
  .hero-description {
    font-size: 1.1rem;
  }
  
  .section-title {
    font-size: 1.8rem;
    margin-bottom: 40px;
  }
  
  .pricing-cards {
    flex-direction: column;
    align-items: center;
  }
  
  .pricing-card {
    width: 100%;
    max-width: 400px;
  }
  
  .footer-links {
    flex-direction: column;
  }
  
  .footer-bottom {
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }
}
</style> 