<script setup></script>

<template>
  <section class="team__section" id="team">
    <div class="team__section-visual">
      <img src="../assets/colorTeam.svg" alt="Рука держащая кисть" />
    </div>
    <div class="team__section-content">
      <h2 class="team__section-title">Наша команда</h2>
      <p class="team__section-description">
        Значимость этих проблем настолько очевидна, что базовый вектор развития позволяет оценить
        значение экспериментов, поражающих по своей масштабности и грандиозности. Мы вынуждены
        отталкиваться от того, что консультация с широким активом.
      </p>
      <div class="team__list">
        <div class="team__list-item">
          <img src="../assets/team1.svg" alt="Член команды 1" />
        </div>
        <div class="team__list-item">
          <img src="../assets/team2.svg" alt="Член команды 2" />
        </div>
        <div class="team__list-item">
          <img src="../assets/team3.svg" alt="Член команды 3" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.team__section {
  display: grid;
  grid-template-columns: 1fr 1fr;
  justify-content: space-between;
  align-items: center;
  max-width: 1110px;
  margin: 0 auto;
  padding: 64px 32px;
  gap: 32px;
}

.team__section-visual {
  max-width: 540px;
  width: 100%;
}

.team__section-content {
  max-width: 540px;
  width: 100%;
  text-align: left;
}

.team__section-title {
  font-family: 'Raleway';
  font-size: 40px;
  font-weight: 500;
  line-height: 110.00000000000001%;
  margin-bottom: 20px;
  color: #2c2d35;
}

.team__section-description {
  font-family: 'Raleway';
  font-size: 18px;
  font-weight: 500;
  line-height: 150%;
  margin-bottom: 20px;
  color: #2c2d35;
}

.team__list {
  display: flex;
  align-items: center;
  gap: 30px;
}

.team__list-item {
  width: 80px;
  height: 80px;
}

@media (max-width: 1024px) {
  .team__section {
    grid-template-columns: 1fr;
    padding: 32px 16px;
  }
}

@media (max-width: 610px) {
  .team__section-visual {
    width: 100%;
  }
}

@media (max-width: 510px) {
  .team__section-content {
    text-align: left;
  }
}
</style>
