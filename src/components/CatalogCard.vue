<script setup>
defineProps({
  image: String,
  author: String,
  title: String,
  description: String,
  price: String,
})
</script>

<template>
  <article class="catalog__card">
    <img :src="image" :alt="title" class="catalog__card-image" />
    <p class="catalog__card-author">{{ author }}</p>
    <h3 class="catalog__card-title">{{ title }}</h3>
    <p class="catalog__card-description">{{ description }}</p>
    <p class="catalog__card-price">{{ price }}</p>
    <button class="catalog__card-button">В корзину</button>
  </article>
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

.catalog__cards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 30px;
}

@media (max-width: 1024px) {
  .catalog__cards {
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
  }
}

@media (max-width: 610px) {
  .catalog__cards {
    grid-template-columns: 1fr;
    gap: 20px;
  }

  .catalog__top {
    flex-direction: column;
    align-items: flex-start;
    gap: 15px;
  }

  .catalog__top-filter {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
  }
}

@media (max-width: 510px) {
  .catalog__cards {
    grid-template-columns: 1fr;
    gap: 15px;
  }

  .catalog__card {
    padding: 15px;
  }

  .catalog__card-title {
    font-size: 16px;
  }

  .catalog__card-price {
    font-size: 14px;
  }

  .catalog__card-button {
    font-size: 14px;
    padding: 8px 12px;
  }
}
</style>
