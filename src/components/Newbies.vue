<script setup></script>

<template>
  <section class="newbies" id="newbies">
    <div class="container">
      <div class="newbies__content">
        <div class="newbies__content-icon-tittle">
          <img src="../assets/Star2.svg" alt="Star" class="newbies__content-icon" />
          <h2 class="newbies__content-title">Новая коллекция французских авторов</h2>
        </div>
        <p class="newbies__content-description">
          Сложно сказать, почему акционеры крупнейших компаний призывают нас к новым свершениям,
          которые, в свою очередь, должны быть заблокированы в рамках своих собственных рациональных
          ограничений.
        </p>
        <p class="newbies__content-description">
          Принимая во внимание показатели успешности, граница обучения кадров предопределяет высокую
          востребованность направлений прогрессивного развития.
        </p>
        <button class="newbies__content-button">Ознакомиться</button>
      </div>
    </div>
  </section>
</template>

<style scoped>
.newbies {
  position: relative;
  background: url('../assets/pic_background.svg');
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  overflow: hidden;
  padding-top: 66px;
  padding-bottom: 73px;
  display: flex;
  align-items: center;
  min-height: 574px;
  margin-bottom: 70px;
}

.container {
  max-width: 1440px;
  padding: 20px 60px;
}

.newbies__content {
  max-width: 540px;
  text-align: left;
}

.newbies__content-icon {
  width: 80px;
  height: 80px;
}

.newbies__content-icon-tittle {
  display: flex;
  align-items: center;
  gap: 20px;
}

.newbies__content-title {
  font-family: 'Raleway';
  font-size: 40px;
  font-weight: 500;
  margin-bottom: 20px;
  color: #f4f6f5;
}

.newbies__content-description {
  font-family: 'Raleway';
  font-size: 18px;
  font-weight: 500;
  margin-bottom: 16px;
  color: #fff;
}

.newbies__content-button {
  font-family: 'Raleway';
  font-size: 20px;
  font-weight: 500;
  line-height: 100%;
  color: #2c2d35;
  background-color: #eedb6d;
  padding: 20px 60px;
  border: none;
  cursor: pointer;
  margin-top: 60px;
}

.newbies__content-button:hover {
  background-color: #e2d693;
  transition: all 0.4s ease-in-out;
}
</style>
