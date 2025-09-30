<script setup>
import { ref } from 'vue'
import CatalogCard from './CatalogCard.vue'
import cardImage1 from '../assets/card1.svg'
import cardImage2 from '../assets/card2.svg'
import cardImage3 from '../assets/card3.svg'
import cardImage4 from '../assets/card4.svg'
import cardImage5 from '../assets/card5.svg'
import cardImage6 from '../assets/card6.svg'
import Germany1 from '../assets/germany1.svg'
import Germany2 from '../assets/germany2.svg'
import Germany3 from '../assets/germany3.svg'
import Germany4 from '../assets/germany4.svg'
import Germany5 from '../assets/germany5.svg'
import Germany6 from '../assets/germany6.svg'
import England1 from '../assets/england.svg'
import England2 from '../assets/england2.svg'
import England3 from '../assets/england3.svg'
import England4 from '../assets/england4.svg'
import England5 from '../assets/england5.svg'
import England6 from '../assets/england6.svg'

const selectedCountry = ref('Франция')
const selectedCategory = ref('Германия')
const selectedCount = ref('Англия')

const cards = [
  {
    country: 'Франция',
    image: cardImage1,
    author: 'Марсель Руссо',
    title: 'Охота Амура',
    description: 'Холст, масло (50х80)',
    price: '14 500 руб',
  },
  {
    country: 'Франция',
    image: cardImage2,
    author: 'Анри Селин',
    title: 'Дама с собачкой',
    description: 'Акрил, бумага (50х80)',
    price: '16 500 руб',
  },
  {
    country: 'Франция',
    image: cardImage3,
    author: 'Франсуа Дюпон',
    title: 'Процедура',
    description: 'Цветная литография (40х60) ',
    price: '20 000 руб',
  },
  {
    country: 'Франция',
    image: cardImage4,
    author: 'Луи Детуш',
    title: 'Роза',
    description: 'Бумага, акрил (50х80) ',
    price: '12 000 руб',
  },
  {
    country: 'Франция',
    image: cardImage5,
    author: 'Франсуа Дюпон',
    title: 'Птичья трапеза',
    description: 'Цветная литография (40х60)',
    price: '22 500 руб',
  },
  {
    country: 'Франция',
    image: cardImage6,
    author: 'Пьер Моранж',
    title: 'Пейзаж с рыбой',
    description: 'Цветная литография (40х60) ',
    price: '22 500 руб',
  },
  {
    country: 'Германия',
    image: Germany1,
    author: 'Курт Вернер',
    title: 'Над городом',
    description: 'Цветная литография (40х60) ',
    price: '16 000 руб',
  },
  {
    country: 'Германия',
    image: Germany2,
    author: 'Макс Рихтер',
    title: 'Птенцы',
    description: 'Холст, масло (50х80) ',
    price: '14 500 руб',
  },
  {
    country: 'Германия',
    image: Germany3,
    author: 'Мартин Майер',
    title: 'Среди листьев',
    description: 'Цветная литография (40х60) ',
    price: '20 000 руб',
  },
  {
    country: 'Германия',
    image: Germany4,
    author: 'Герман Беккер',
    title: 'Яркая птица',
    description: 'Цветная литография (40х60) ',
    price: '13 000 руб',
  },
  {
    country: 'Германия',
    image: Germany5,
    author: 'Вульф Бауэр',
    title: 'Дятлы',
    description: 'Бумага, акрил (50х80) ',
    price: '20 000 руб',
  },
  {
    country: 'Германия',
    image: Germany6,
    author: 'Вальтер Хартманн',
    title: 'Большие воды',
    description: 'Бумага, акрил (50х80) ',
    price: '23 000 руб',
  },
  {
    country: 'Англия',
    image: England1,
    author: 'Пол Смит',
    title: 'Дикий зверь',
    description: 'Акварель, бумага (50х80) ',
    price: '19 500 руб',
  },
  {
    country: 'Англия',
    image: England2,
    author: 'Джон Уайт',
    title: 'Скалистый берег',
    description: 'Цветная литография (40х60) ',
    price: '17 500 руб',
  },
  {
    country: 'Англия',
    image: England3,
    author: 'Джим Уотсон',
    title: 'Река и горы',
    description: 'Акварель, бумага (50х80) ',
    price: '20 500 руб',
  },
  {
    country: 'Англия',
    image: England4,
    author: 'Юджин Зиллион',
    title: 'Белый попугай',
    description: 'Цветная литография (40х60)',
    price: '15 500 руб',
  },
  {
    country: 'Англия',
    image: England5,
    author: 'Эрик Гиллман',
    title: 'Ночная рыба',
    description: 'Бумага, акрил (50х80) ',
    price: '12 500 руб',
  },
  {
    country: 'Англия',
    image: England6,
    author: 'Альфред Барр',
    title: 'Рыжий кот',
    description: 'Цветная литография (40х60) ',
    price: '21 000 руб',
  },
]

const filteredCards = () => cards.filter((card) => card.country === selectedCountry.value)
</script>
<template>
  <section class="catalog" id="catalog">
    <div class="catalog__top">
      <h2 class="catalog__top-title">Репродукции</h2>
      <div class="catalog__top-filter">
        <button
          class="catalog__top-filter-button"
          :class="{ 'catalog__top-filter-button--active': selectedCountry === 'Франция' }"
          @click="selectedCountry = 'Франция'"
        >
          Франция
        </button>
        <button
          class="catalog__top-filter-button"
          :class="{ 'catalog__top-filter-button--active': selectedCountry === 'Германия' }"
          @click="selectedCountry = 'Германия'"
        >
          Германия
        </button>
        <button
          class="catalog__top-filter-button"
          :class="{ 'catalog__top-filter-button--active': selectedCountry === 'Англия' }"
          @click="selectedCountry = 'Англия'"
        >
          Англия
        </button>
      </div>
    </div>
    <div class="catalog__cards">
      <CatalogCard
        v-for="(card, index) in filteredCards()"
        :key="index"
        :image="card.image"
        :author="card.author"
        :title="card.title"
        :description="card.description"
        :price="card.price"
      />
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
