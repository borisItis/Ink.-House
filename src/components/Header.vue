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
  padding: 20px 165px;
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
  color: #86928b;
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
    padding: 20px 32px;
  }
  .nav__right {
    gap: 32px;
  }
  .nav__list {
    gap: 32px;
  }
}

@media (max-width: 510px) {
  .nav {
    padding: 15px;
  }
  .header {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
    padding: 15px;
  }

  .header__logo {
    margin-bottom: 10px;
    font-size: 18px;
  }

  .header__nav {
    display: flex;
    justify-content: center;
    gap: 20px;
    order: 2;
  }

  .nav__list-item {
    font-size: 18px;
  }

  .header__cart {
    margin-left: 15px;
    width: 20px;
    height: 20px;
  }

  .header__bottom {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
  }
}
</style>
