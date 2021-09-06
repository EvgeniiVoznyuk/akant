<template>
  <div class="footer">
    <div class="footer__container container">
      <div class="footer__left">
        <img src="~@/assets/img/akantFooter.svg" />
        <div class="footer__icons">
          <img src="~@/assets/img/facebook.svg" />
          <img src="~@/assets/img/instagram.svg" />
          <img src="~@/assets/img/telegram.svg" />
        </div>
      </div>
      <div class="footer__right">
        <ul class="footer__list">
          <h1 class="footer__list-title">Главная</h1>
          <li class="footer__list-item">Направления обучения</li>
          <li class="footer__list-item">Как проходит обучение</li>
          <li class="footer__list-item">Атмосфера обучения</li>
          <li class="footer__list-item">Наши преподаватели</li>
          <li class="footer__list-item">Работы кураторов</li>
          <li class="footer__list-item">Отзывы</li>
        </ul>

        <ul class="footer__list">
          <h1 class="footer__list-title">Где нас найти</h1>
          <li class="footer__list-item">г. Киев</li>
        </ul>

        <ul class="footer__list">
          <h1 class="footer__list-title">Контакты</h1>
          <li class="footer__list-item">akant@gmail.com</li>
          <li class="footer__list-item">+380 *** ** **</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.footer {
  padding: 50px 20px;
  height: 420px;
  background-color: #000;
  display: flex;
  justify-content: center;

  &__container {
    display: flex;
    justify-content: space-around;
  }

  &__left {
    display: flex;
    flex-direction: column;
    gap: 30px;
    align-items: start;
  }

  &__right {
    display: flex;
    gap: 70px;
  }

  &__icons {
    display: flex;
    gap: 30px;
    cursor: pointer;
  }

  &__list {
    color: #fff;
    font-family: "Roboto";
    font-size: 18px;

    &-title {
      font-weight: medium;
      padding-bottom: 30px;
      cursor: pointer;
    }

    &-item {
      font-weight: 400;
      line-height: 22px;
      padding-bottom: 20px;
      cursor: pointer;

      &:hover {
      color: rgb(230, 153, 53);
    }
    }
  }
}
</style>
