<template>
  <div class="about-page">
    <br/><br/><br/>
   
    <div class="about-content">
      <div class="sobre-nos-box">
        <h2 class="sobre-nos-title">Quem somos nós?</h2>
        <p class="sobre-nos-text">
          Somos um grupo de estudantes do 3º ano do ensino médio, com foco em veterinária e zootecnia. Nosso projeto, "Vetz", busca explorar de forma inovadora a relação entre os animais, a saúde deles e a acessibilidade. Com foco em áreas como comportamento animal, controle de vacinação e práticas de cuidado, unindo conhecimento e sensibilidade para transformar a forma como lidamos com os nossos animais.<br>
          Nosso objetivo é contribuir para o bem-estar dos animais, de forma que possamos juntar o carinho e cuidado por eles no VetZ.
        </p>
      </div>



     
      <div class="team-section">
       
        <div class="team-grid">
          <div v-for="member in team" :key="member.id" class="team-member">
            <div class="member-avatar">{{ member.emoji }}</div>
            <h3>{{ member.name }}</h3>
            <p class="member-role">{{ member.role }}</p>
          </div>
        </div>
      </div>

      <div class="values-section">
       
        <div class="values-list">
          <div v-for="value in values" :key="value.id" class="value-item">
            <span class="value-icon">{{ value.icon }}</span>
            <div>
              <h4>{{ value.title }}</h4>
              <p>{{ value.description }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const stats = ref({
  years: 5,
  projects: 150,
  clients: 89
})






</script>

<style scoped>
.about-page {
  width: 100vw;
  min-height: 100vh;
  background-color: #FEFFEF;
  margin: 0;
  padding: 0;
}

.about-content {
  text-align: left;
}

.company-info {
  background-color: #FEFFEF;
  box-shadow: none;
  border-radius: 0;
  padding: 48px 0 32px 0;
  margin-bottom: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.sobre-nos-box {
  background: #fff;
  border-radius: 4px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.10);
  padding: 96px 96px 72px 96px;
  margin: 24px auto 32px auto;
  max-width: 95vw;
  width: 900px;
}
.sobre-nos-title {
  font-size: 1.4rem;
  font-weight: 600;
  color: #222;
  margin-bottom: 16px;
}
.sobre-nos-text {
  font-size: 1.18rem;
  color: #222;
  line-height: 1.6;
  margin: 0;
}
/* Título maior */
.about-title {
  font-size: 2.7rem;
  font-weight: bold;
  color: #007bff;
  margin-bottom: 25px;
  text-align: center;
}

/* Texto principal maior */
.about-text {
  font-size: 1.35rem;
  line-height: 2.1;
  color: #333;
  text-align: center;
  max-width: 900px;
}

.company-info h2 {
  color: #495057;
  margin-bottom: 15px;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 20px;
  margin-bottom: 40px;
}

.stat-card {
  background-color: white;
  border: 2px solid #007bff;
  border-radius: 8px;
  padding: 20px;
  text-align: center;
}

.stat-number {
  font-size: 2.5rem;
  font-weight: bold;
  color: #007bff;
}

.stat-label {
  color: #6c757d;
  font-size: 0.9rem;
  margin-top: 5px;
}

.team-section {
  margin-bottom: 40px;
}

.team-section h2 {
  color: #495057;
  margin-bottom: 20px;
}

.team-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 20px;
}

.team-member {
  background-color: white;
  border: 1px solid #dee2e6;
  border-radius: 8px;
  padding: 20px;
  text-align: center;
}

.member-avatar {
  font-size: 3rem;
  margin-bottom: 10px;
}

.team-member h3 {
  color: #495057;
  margin-bottom: 5px;
}

.member-role {
  color: #6c757d;
  font-size: 0.9rem;
}

.values-section h2 {
  color: #495057;
  margin-bottom: 20px;
}

.values-list {
  display: grid;
  gap: 15px;
}

.value-item {
  display: flex;
  align-items: flex-start;
  background-color: #f8f9fa;
  padding: 20px;
  border-radius: 8px;
  border-left: 4px solid #007bff;
}

.value-icon {
  font-size: 2rem;
  margin-right: 15px;
}

.value-item h4 {
  color: #495057;
  margin-bottom: 5px;
}

.value-item p {
  color: #6c757d;
  margin: 0;
}
</style>
