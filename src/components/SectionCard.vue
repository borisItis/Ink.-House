<script setup></script>

<template>
  <section class="catalog" id="catalog">
    <div class="catalog__top">
      <h2 class="catalog__top-title">Репродукции</h2>
      <div class="catalog__top-filter">
        <button class="catalog__top-filter-button catalog__top-filter-button--active">
          Франция
        </button>
        <button class="catalog__top-filter-button">Германия</button>
        <button class="catalog__top-filter-button">Англия</button>
      </div>
    </div>
    <div class="catalog__cards">
      <article class="catalog__card">
        <img src="../assets/card1.svg" alt="Охота Амура" class="catalog__card-image" />
        <p class="catalog__card-author">Марсель Руссо</p>
        <h3 class="catalog__card-title">Охота Амура</h3>
        <p class="catalog__card-description">Холст, масло (50х80)</p>
        <p class="catalog__card-price">14 500 руб</p>
        <button class="catalog__card-button">В корзину</button>
      </article>
      <article class="catalog__card">
        <img src="../assets/card2.svg" alt="Охота Амура" class="catalog__card-image" />
        <p class="catalog__card-author">Анри Селин</p>
        <h3 class="catalog__card-title">Дама с собачкой</h3>
        <p class="catalog__card-description">Акрил, бумага (50х80)</p>
        <p class="catalog__card-price">16 500 руб</p>
        <button class="catalog__card-button">В корзину</button>
      </article>
      <article class="catalog__card">
        <img src="../assets/card3.svg" alt="Охота Амура" class="catalog__card-image" />
        <p class="catalog__card-author">Франсуа Дюпон</p>
        <h3 class="catalog__card-title">Процедура</h3>
        <p class="catalog__card-description">Цветная литография (40х60)</p>
        <p class="catalog__card-price">20 000 руб</p>
        <button class="catalog__card-button">В корзину</button>
      </article>
      <article class="catalog__card">
        <img src="../assets/card4.svg" alt="Охота Амура" class="catalog__card-image" />
        <p class="catalog__card-author">Луи Детуш</p>
        <h3 class="catalog__card-title">Роза</h3>
        <p class="catalog__card-description">Бумага, акрил (50х80)</p>
        <p class="catalog__card-price">12 000 руб</p>
        <button class="catalog__card-button">В корзину</button>
      </article>
      <article class="catalog__card">
        <img src="../assets/card5.svg" alt="Охота Амура" class="catalog__card-image" />
        <p class="catalog__card-author">Франсуа Дюпон</p>
        <h3 class="catalog__card-title">Птичья трапеза</h3>
        <p class="catalog__card-description">Цветная литография (40х60)</p>
        <p class="catalog__card-price">22 500 руб</p>
        <button class="catalog__card-button">В корзину</button>
      </article>
      <article class="catalog__card">
        <img src="../assets/card6.svg" alt="Охота Амура" class="catalog__card-image" />
        <p class="catalog__card-author">Пьер Моранж</p>
        <h3 class="catalog__card-title">Пейзаж с рыбой</h3>
        <p class="catalog__card-description">Цветная литография (40х60)</p>
        <p class="catalog__card-price">20 000 руб</p>
        <button class="catalog__card-button">В корзину</button>
      </article>
    </div>
  </section>
</template>

<style scoped>
.catalog {
  max-width: 1110px;
  margin: 0 auto;
  padding: 64px 32px;
}

.catalog__top {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 32px;
  margin-bottom: 30px;
}

.catalog__top-title {
  font-family: 'Raleway';
  font-size: 40px;
  font-weight: 500;
  margin-bottom: 30px;
  color: #2c2d35;
}

.catalog__top-filter {
  display: flex;
  align-items: center;
  gap: 32px;
}

.catalog__top-filter-button {
  font-family: 'Raleway';
  font-size: 20px;
  font-weight: 500;
  color: #2c2d35;
  padding: 10px 20px;
  border-radius: 20px;
  background-color: #d4e8d9;
  border: none;
  cursor: pointer;
}

.catalog__top-filter-button--active {
  background-color: #376b44;
  color: white;
}

.catalog__top-filter-button:hover {
  background-color: #598;
  color: white;
  transition: all 0.4s ease-in-out;
}

.catalog__cards {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 30px;
}

.catalog__card {
  background-color: #e1ede6;
  padding: 20px;
  display: flex;
  flex-direction: column;
}

.catalog__card-image {
  width: 100%;
  height: auto;
  display: block;
  margin-bottom: 20px;
}

.catalog__card-author {
  font-family: 'Raleway';
  font-size: 18px;
  font-weight: 500;
  margin-bottom: 10px;
  color: #86928b;
}

.catalog__card-title {
  font-family: 'Raleway';
  font-size: 30px;
  font-weight: 500;
  margin-bottom: 8px;
  color: #2c2d35;
}

.catalog__card-description {
  font-family: 'Raleway';
  font-size: 18px;
  font-weight: 500;
  margin-bottom: 30px;
  color: #2c2d35;
}

.catalog__card-price {
  font-family: 'Raleway';
  font-size: 24px;
  font-weight: 500;
  margin-bottom: 20px;
  color: #598d66;
}

.catalog__card-button {
  font-family: 'Raleway';
  font-size: 20px;
  font-weight: 500;
  line-height: 100%;
  color: #598d66;
  background-color: transparent;
  padding: 20px 60px;
  border: 1px solid #598d66;
  cursor: pointer;
  margin-bottom: 30px;
}

.catalog__card-button:hover {
  background-color: #598d66;
  color: white;
  transition: all 0.4s ease-in-out;
}
</style>
