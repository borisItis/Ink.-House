<script setup></script>

<template>
  <nav class="nav">
    <a href="" class="nav__logo">
      <img src="../assets/logo.svg" class="nav__logo-img" alt="" />
    </a>
    <div class="nav__right">
      <ul class="nav__list">
        <li class="nav__list-item"><a href="#catalog"></a>Репродукции</li>
        <li class="nav__list-item"><a href="#newbies"></a>Новинки</li>
        <li class="nav__list-item"><a href="#team"></a>О нас</li>
      </ul>
      <button class="nav__button">
        <img src="../assets/cart.svg" alt="" />
      </button>
    </div>
  </nav>
</template>

<style scoped>
nav {
  background-color: #e1ede6;
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1440px;
  width: 100%;
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
}

.nav__list-item {
  cursor: pointer;
  font-size: 20px;
  line-height: 100%;
  font-weight: 500;
  padding: 4px;
  color: #2c2d35;
}

.nav__list-item:hover {
  color: #e1ede6;
  transition: all 0.4s ease;
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
</style>
