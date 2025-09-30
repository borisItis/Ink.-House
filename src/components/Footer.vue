<script setup></script>

<template>
  <footer class="footer">
    <div class="footer__container">
      <div class="footer__info">
        <a href="#!" class="footer__info-logo">
          <img src="../assets/logo.svg" alt="Logo" />
        </a>
        <div class="footer__info-contacts">
          <a href="tel:+7 (999) 543-54-54" class="footer__info-phone">+7 (999) 543-54-54</a>
          <h6 class="footer__info-subtitle">Мастерская</h6>
        </div>
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

.footer__info-contacts {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
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
  align-items: center;
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
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 30px;
}

.footer__socials-icon {
  display: flex;
  align-items: center;
  width: 24px;
  height: 24px;
}

.footer__socials-icon:hover {
  transform: scale(1.05);
}

.footer__socials-copyright {
  font-size: 12px;
  opacity: 0.7;
  line-height: 1.4;
  text-align: left;
  flex-shrink: 0;
  margin: 0;
}

@media (max-width: 1024px) {
  .footer__container {
    grid-template-columns: 1fr 1fr 1fr;
    gap: 25px;
  }

  .footer__socials {
    grid-column: 1 / -1;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    margin-top: 20px;
    padding-top: 20px;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
  }

  .footer__socials-icon {
    margin-bottom: 0;
    margin-right: 20px;
  }

  .footer__socials-copyright {
    margin-top: 0;
    text-align: center;
  }
}

@media (max-width: 610px) {
  .footer__container {
    grid-template-columns: 1fr 1fr;
    gap: 30px 20px;
  }

  .footer__info {
    grid-column: 1 / -1;
    text-align: center;
    margin-bottom: 10px;
  }

  .footer__socials {
    grid-column: 1 / -1;
    flex-direction: column;
    align-items: center;
    text-align: center;
    margin-top: 10px;
  }

  .footer__socials-icon {
    margin-right: 0;
    margin-bottom: 15px;
    margin-right: 15px;
    display: inline-block;
  }

  .footer__socials-copyright {
    text-align: center;
    margin-top: 10px;
  }
}

@media (max-width: 510px) {
  .footer {
    padding: 30px 0;
  }

  .footer__container {
    grid-template-columns: 1fr;
    gap: 25px;
    text-align: center;
  }

  .footer__info {
    grid-column: 1;
  }

  .footer__menu {
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    padding-bottom: 15px;
  }

  .footer__menu:last-child {
    border-bottom: none;
  }

  .footer__socials {
    grid-column: 1;
    flex-direction: row;
    justify-content: center;
    flex-wrap: wrap;
  }

  .footer__socials-icon {
    margin: 0 10px 10px;
  }

  .footer__socials-copyright {
    width: 100%;
    margin-top: 10px;
  }
}
</style>
