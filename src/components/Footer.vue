<script setup></script>

<template>
  <footer class="footer">
    <div class="footer__container">
      <div class="footer__info">
        <a href="#!" class="footer__info-logo">
          <img src="../assets/logo.svg" alt="Logo" />
        </a>
        <a href="tel:+7 (999) 543-54-54" class="footer__info-phone">+7 (999) 543-54-54</a>
        <h6 class="footer__info-subtitle">Мастерская</h6>
      </div>
      <div class="footer__menu">
        <h4 class="footer__menu-title">Репродукции</h4>
        <ul class="footer__menu-list">
          <li class="footer__menu-item"><a href="#!" class="footer__menu-link">Франция</a></li>
          <li class="footer__menu-item"><a href="#!" class="footer__menu-link">Германия</a></li>
          <li class="footer__menu-item"><a href="#!" class="footer__menu-link">Англия</a></li>
        </ul>
      </div>
      <div class="footer__menu">
        <h4 class="footer__menu-title">Новинки</h4>
        <ul class="footer__menu-list">
          <li class="footer__menu-item"><a href="#!" class="footer__menu-link">2021</a></li>
          <li class="footer__menu-item"><a href="#!" class="footer__menu-link">2020</a></li>
        </ul>
      </div>
      <div class="footer__menu">
        <h4 class="footer__menu-title">О нас</h4>
        <ul class="footer__menu-list">
          <li class="footer__menu-item"><a href="#!" class="footer__menu-link">Художники</a></li>
          <li class="footer__menu-item"><a href="#!" class="footer__menu-link">Менеджеры</a></li>
        </ul>
      </div>
      <div class="footer__socials">
        <a href="#!" class="footer__socials-icon">
          <img src="../assets/facebook.svg" alt="FaceBook" />
        </a>
        <a href="#!" class="footer__socials-icon">
          <img src="../assets/instagram.svg" alt="Instagram" />
        </a>
        <a href="#!" class="footer__socials-icon">
          <img src="../assets/youtube.svg" alt="YouTube" />
        </a>
        <p class="footer__socials-copyright">Ink. House ®<br />All rights reserved</p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  padding-top: 23px;
  padding-bottom: 23px;
  background-color: #e1ede6;
}

.footer__container {
  max-width: 1440px;
  display: flex;
  margin: 0 auto;
  justify-content: space-between;
}

.footer__info {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.footer__info-logo {
  display: inline-block;
  margin-bottom: 35px;
}

.footer__info-phone {
  font-family: 'Raleway';
  font-size: 20px;
  font-weight: 500;
  color: #2c2d35;
  text-decoration: none;
}

.footer__info-subtitle {
  font-family: 'Raleway';
  font-size: 18px;
  font-weight: 500;
  color: #86928b;
}

.footer__menu {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.footer__menu-title {
  font-family: 'Raleway';
  font-size: 20px;
  font-weight: 500;
  color: #2c2d35;
  margin-bottom: 6px;
}

.footer__menu-list {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 6px;
  list-style: none;
}

.footer__menu-link {
  text-decoration: none;
  color: #376b44;
  font-size: 18px;
  line-height: 150%;
  font-weight: 500;
}

.footer__menu-link:hover {
  color: #86928b;
}

.footer__socials {
  display: flex;
  gap: 30px;
}

.footer__socials-icon {
  align-items: center;
  width: 24px;
  height: 24px;
}

.footer__socials-icon:hover {
  transform: scale(1.05);
}

.footer__socials-copyright {
  margin-top: 57px;
  font-family: 'Raleway';
  font-size: 12px;
  font-weight: 500;
  color: #86928b;
  line-height: 120%;
}
</style>
