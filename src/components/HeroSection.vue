<script setup></script>

<template>
  <section class="hero">
    <div class="hero__image">
      <img src="../assets/heroImage.svg" alt="" />
    </div>
    <div class="hero__content">
      <h1 class="hero__title">Реплики картин от <span>Ink. House</span></h1>
      <p class="hero__description">
        Высокое качество отрисовки на плотной бумаге или льняном холсте. Редкие произведения,
        доступные цены.
      </p>
      <button class="hero__button">Продукция</button>
    </div>
  </section>
</template>

<style scoped>
.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1440px;
  padding: 64px 32px;
  margin: 0 auto;
}

.hero__content {
  max-width: 540px;
  padding-right: 165px;
}

.hero__title {
  font-family: 'Raleway';
  font-size: 60px;
  font-weight: 500;
  line-height: 110.00000000000001%;
  margin-bottom: 20px;
}

.hero__title span {
  font-family: 'Raleway';
  font-size: 60px;
  line-height: 110.00000000000001%;
  color: #598d66;
}

.hero__description {
  font-family: 'Raleway';
  font-size: 18px;
  font-weight: 500;
  line-height: 150%;
  color: #86928b;
  margin-bottom: 60px;
}

.hero__button {
  font-family: 'Raleway';
  font-size: 20px;
  font-weight: 500;
  line-height: 100%;
  color: #598d66;
  background-color: transparent;
  padding: 20px 60px;
  border: 1px solid #598d66;
  cursor: pointer;
}

.hero__button:hover {
  background-color: #598d66;
  color: white;
  transition: all 0.4s ease-in-out;
}

.hero__image {
  max-width: 540px;
  width: 100%;
  margin-left: 165px;
}

@media (max-width: 1024px) {
  .hero {
    flex-direction: column;
    padding: 32px 16px;
  }
  .hero__content {
    padding-right: 0px;
    text-align: center;
  }
  .hero__image {
    margin-left: 0px;
    margin-top: 32px;
  }
}

@media (max-width: 690px) {
  .hero {
    flex-direction: column;
    padding: 32px 16px;
  }
  .hero__content {
    padding-right: 0px;
    text-align: center;
  }
  .hero__image {
    margin-left: 0px;
    margin-top: 32px;
  }
}

@media (max-width: 510px) {
  .hero {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    padding: 20px 10px;
  }

  .hero__image {
    width: 100%;
    margin-bottom: 15px;
  }

  .hero__title {
    line-height: 1.3;
    margin-bottom: 10px;
  }

  .hero__text {
    font-size: 14px;
    line-height: 1.4;
    margin-bottom: 15px;
  }

  .hero__button {
    font-size: 14px;
    padding: 10px 18px;
  }
}
</style>
