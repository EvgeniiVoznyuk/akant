<template>
  <header class="header">
    <div class="header__container container">
      <div class="header__title-group">
        <img class="header__akant" src="~@/assets/img/akant.png" />
        <h1 class="header__title montserrat">
          Школа дизайна и творчества <span class="akant">Акант</span>
        </h1>
      </div>
      <div class="navbar">
        <ul class="navbar__list">
          <li class="navbar__item">О школе</li>
          <li class="navbar__item">Ближайший набор</li>
          <li class="navbar__item">Отзывы</li>
          <li class="navbar__item">Портфолио</li>
          <li class="navbar__item">Наши преимущества</li>
          <li class="navbar__item">Контакты</li>
        </ul>
      </div>
      <button class="btn montserrat">Начать обучение с нами</button>
    </div>
  </header>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.header {
  display: flex;
  justify-content: center;
  background-image: url("~@/assets/img/firstScreen.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  padding: 0 30px 40px 0;

  &__title-group {
    display: flex;
    align-items: flex-start;
    justify-content: center;
    gap: 20px;
  }

  &__akant {
    height: 500px;
  }
  
  &__container {
    display: flex;
    flex-direction: column;
  };

  &__title {
    margin-top: 20px;
    display: flex;
    align-items: center;
    width: 65%;
    padding: 30px 40px 30px 30px;
    background-color: rgba(#000, 0.44);

    font-size: 36px;
    color: #fff;

    .akant {
      padding-left: 30px;
      font-size: 72px;
      line-height: 82px;
      text-transform: uppercase;
    }
  }
}
.navbar {
  margin-top: 10px;
  padding: 30px 20px;
  background-color: rgba(#000, 0.44);
  align-self: center;

  &__list {
    display: flex;
    gap: 50px;
    font-family: "Montserrat", serif;
    font-size: 20px;
    color: #fff;
  };

  &__item {
    cursor: pointer;

    &:hover {
      color: rgb(230, 153, 53);
    }
  }
}

</style>
