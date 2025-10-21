<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}
</script>

<template>
  <nav class="nav">
    <a href="" class="nav__logo">
      <img src="../assets/logo.svg" class="nav__logo-img" alt="" />
    </a>
    <div class="nav__right">
      <button class="nav__menu-button" @click="toggleMenu">
        <img v-if="!isMenuOpen" src="../assets/burger.svg" alt="open menu" />
        <img v-else src="../assets/close.svg" alt="close menu" />
      </button>
      <ul class="nav__list" :class="{ 'nav__list--open': isMenuOpen }">
        <li class="nav__list-item"><a href="#catalog">Репродукции</a></li>
        <li class="nav__list-item"><a href="#newbies">Новинки</a></li>
        <li class="nav__list-item"><a href="#team">О нас</a></li>
      </ul>
      <button class="nav__button">
        <img src="../assets/cart.svg" alt="cart" />
      </button>
    </div>
  </nav>
</template>

<style scoped>
header {
  width: 100%;
}

nav {
  max-width: 1440px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #e1ede6;
  padding: 20px;
  margin: 0 auto;
  gap: 8px;
}

.nav__logo {
  max-width: 143px;
  width: 100%;
}

.nav__logo-img {
  width: 100%;
}

.nav__right {
  display: flex;
  align-items: center;
  gap: 60px;
}

.nav__list {
  display: flex;
  list-style: none;
  gap: 60px;
  margin: 0;
  padding: 0;
}

.nav__list-item a {
  cursor: pointer;
  font-size: 20px;
  font-family: 'Raleway';
  text-decoration: none;
  line-height: 100%;
  font-weight: 500;
  padding: 4px;
  color: #2c2d35;
  transition: all 0.4s ease;
}

.nav__list-item a:hover {
  color: #86928b;
}

.nav__menu-button {
  display: none;
}

.nav__button {
  background-color: transparent;
  border: none;
  cursor: pointer;
  padding: 4px;
}

.nav__button:hover {
  color: #e1ede6;
  transition: all 0.4s ease;
}

@media (max-width: 1024px) {
  .nav {
    padding: 20px 32px;
  }
  .nav__right {
    gap: 32px;
  }
  .nav__list {
    gap: 32px;
  }
}

@media (max-width: 690px) {
  .nav {
    flex-direction: column;
    align-items: center;
    padding: 16px 32px;
    gap: 16px;
  }

  .nav__logo {
    order: 1;
    margin-bottom: 8px;
  }

  .nav__right {
    order: 2;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    gap: 24px;
  }

  .nav__list {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 32px;
    margin: 0;
    padding: 0;
  }

  .nav__button {
    margin-left: auto;
  }
}
@media (max-width: 480px) {
  .nav {
    flex-direction: column;
    align-items: center;
    padding: 16px;
    gap: 12px;
  }

  .nav__logo {
    order: 1;
  }

  .nav__right {
    order: 2;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    background-color: #e1ede6;
    padding: 12px 20px;
    border-radius: 6px;
  }

  .nav__list {
    display: none;
    flex-direction: column;
    align-items: flex-start;
    width: 100%;
    background-color: #e1ede6;
    gap: 16px;
    margin-top: 12px;
    padding: 16px 0;
    border-top: 1px solid #c8d5ce;
    transition: all 0.3s ease;
  }

  .nav__menu-button {
    display: block;
    background: none;
    border: none;
    cursor: pointer;
    width: 28px;
    height: 28px;
  }

  .nav__menu-button img {
    width: 100%;
    height: auto;
  }

  .nav__list--open {
    display: flex;
  }

  .nav__list-item a {
    text-decoration: none;
    color: #2c2d35;
    font-size: 18px;
    font-weight: 500;
  }

  .nav__list-item a:hover {
    color: #86928b;
  }

  .nav__button {
    background: none;
    border: none;
    cursor: pointer;
    width: 28px;
    height: 28px;
  }

  .nav__button img {
    width: 100%;
    height: auto;
  }
}
</style>
