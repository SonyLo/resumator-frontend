<template>
  <div class="about">
    <div class="about-content">
      <h1>О конструкторе резюме <span class="gradient-text">Resumator</span></h1>
      <p>
        Resumator - это современный инструмент для создания профессиональных резюме с возможностью
        автоматического размещения на персональном поддомене.
      </p>
      <p>
        Наша миссия - помочь каждому соискателю создать идеальное резюме, которое
        выделит его среди других кандидатов и повысит шансы на получение работы мечты.
      </p>
      <router-link to="/" class="back-link">Вернуться на главную</router-link>
    </div>
  </div>
</template>

<style scoped>
.about {
  min-height: 90vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(180deg, #f8f9fa 0%, #ffffff 100%);
  padding: 20px;
}

.about-content {
  max-width: 800px;
  text-align: center;
}

h1 {
  font-size: 2.5rem;
  margin-bottom: 30px;
  font-weight: 700;
}

.gradient-text {
  background: linear-gradient(90deg, #4776E6 0%, #8E54E9 100%);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
  font-weight: bold;
}

p {
  font-size: 1.2rem;
  line-height: 1.8;
  color: #555;
  margin-bottom: 20px;
}

.back-link {
  display: inline-block;
  margin-top: 30px;
  padding: 12px 28px;
  background: linear-gradient(90deg, #4776E6 0%, #8E54E9 100%);
  color: white;
  text-decoration: none;
  font-weight: 600;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(71, 118, 230, 0.3);
  transition: all 0.3s ease;
}

.back-link:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 16px rgba(71, 118, 230, 0.4);
}
</style>
