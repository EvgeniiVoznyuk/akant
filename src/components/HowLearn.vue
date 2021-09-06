<template>
  <div class="hl">
    <div class="hl__container container">
      <SectionTitle :title="'Как проходит обучение'" />
      <div class="hl__grid grid">
        <div class="grid__item">
          <img
            src="~@/assets/img/gridImages/online.svg"
            class="grid__item-img"
          />
          <h1 class="grid__item-title">Онлайн</h1>
          <p class="grid__item-description">
            Навчання проходить повність онлайн. Всі матеріали зібрані в
            телеграм-каналі, доступ до якого ви матимете і після навчання.
            Лекції проходять на платформі зум.
          </p>
        </div>

        <div class="grid__item">
          <img
            src="~@/assets/img/gridImages/clock.svg"
            class="grid__item-img"
          />
          <h1 class="grid__item-title">Комфортный темп обучение</h1>
          <p class="grid__item-description">
            Навчання проходить повність онлайн. Всі матеріали зібрані в
            телеграм-каналі, доступ до якого ви матимете і після навчання.
            Лекції проходять на платформі зум.
          </p>
        </div>

        <div class="grid__item">
          <img
            src="~@/assets/img/gridImages/support.svg"
            class="grid__item-img"
          />
          <h1 class="grid__item-title">Постоянная поддержка куратора</h1>
          <p class="grid__item-description">
            Навчання проходить повність онлайн. Всі матеріали зібрані в
            телеграм-каналі, доступ до якого ви матимете і після навчання.
            Лекції проходять на платформі зум.
          </p>
        </div>

        <div class="grid__item">
          <img src="~@/assets/img/gridImages/hts.svg" class="grid__item-img" />
          <h1 class="grid__item-title">Разбор домашних заданий</h1>
          <p class="grid__item-description">
            Навчання проходить повність онлайн. Всі матеріали зібрані в
            телеграм-каналі, доступ до якого ви матимете і після навчання.
            Лекції проходять на платформі зум.
          </p>
        </div>

        <div class="grid__item">
          <img
            src="~@/assets/img/gridImages/clock.svg"
            class="grid__item-img"
          />
          <h1 class="grid__item-title">Практики</h1>
          <p class="grid__item-description">
            Навчання проходить повність онлайн. Всі матеріали зібрані в
            телеграм-каналі, доступ до якого ви матимете і після навчання.
            Лекції проходять на платформі зум.
          </p>
        </div>

        <div class="grid__item">
          <img
            src="~@/assets/img/gridImages/diploma.svg"
            class="grid__item-img"
          />
          <h1 class="grid__item-title">Диплом после окончания</h1>
          <p class="grid__item-description">
            Навчання проходить повність онлайн. Всі матеріали зібрані в
            телеграм-каналі, доступ до якого ви матимете і після навчання.
            Лекції проходять на платформі зум.
          </p>
        </div>
      </div>
      <div class="atmosphere">
        <SectionTitle :title="'Атмосфера мастерской'" />
        <div class="atmosphere__container">
          <div class="atmosphere__text-group">
            <h1 class="atmosphere__title">
              Наша школа - место развития для тех, кто хочет максимально
              расскрыть свой творческий потенциал
            </h1>
            <p class="atmosphere__description">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quis
              exercitationem in et corporis assumenda incidunt perferendis sint
              molestiae quidem placeat accusantium excepturi quod nemo ab
              dolorem ad aliquid facere, labore atque ipsum maxime. Quas,
              deserunt! Repudiandae vero eum exercitationem reiciendis earum
              atque delectus praesentium mollitia? Porro totam reprehenderit
              quis? Quidem, voluptate nemo animi nam iure nisi quae expedita
              error aliquam hic omnis dolorem magnam consequatur. Blanditiis
              consequuntur soluta fugit ex.
            </p>
          </div>
          <div class="atmosphere__imgs">
            <img src="~@/assets/img/atmosphere/1.png" class="atmosphere__img" />
            <div class="atmosphere__imgs-group atmosphere__imgs-group--1">
              <img
                src="~@/assets/img/atmosphere/2.png"
                class="atmosphere__img"
              />
              <img
                src="~@/assets/img/atmosphere/3.png"
                class="atmosphere__img"
              />
            </div>
            <div class="atmosphere__imgs-group atmosphere__imgs-group--2">
              <img
                src="~@/assets/img/atmosphere/4.png"
                class="atmosphere__img"
              />
              <img
                src="~@/assets/img/atmosphere/5.png"
                class="atmosphere__img"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
/* eslint-disable vue/no-unused-components */
import SectionTitle from "./SectionTitle.vue";
export default {
  components: {
    SectionTitle,
  },
};
</script>

<style lang="scss">
.atmosphere {
  width: 100%;
  padding-top: 150px;
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 70px;

  &__text-group {
    padding: 20px 30px 0;
    display: flex;
    gap: 120px;
    position: relative;
    top: 40px;
  }

  &__title {
    width: 620px;
    font-family: "Montserrat";
    font-size: 20px;
    line-height: 26px;
  }

  &__description {
    width: 500px;
    font-family: "Montserrat";
    font-weight: 400;
    line-height: 24px;
  }

  &__imgs {
    display: flex;
    gap: 20px;

    &-group {
      &--1 {
        padding-top: 70px;
      }
      &--2 {
        padding-top: 110px;
      }
    }
  }
}
.hl {
  height: auto;
  padding-bottom: 50px;
  background-image: url("~@/assets/img/howLearnBg.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  display: flex;
  justify-content: center;

  &__container {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 50px;
  }
}
.grid {
  padding-top: 90px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 90px;

  &__item {
    width: 340px;
    display: flex;
    gap: 25px;
    flex-direction: column;
    align-items: center;

    &-title {
      text-align: center;
      font-family: "Roboto";
      font-size: 20px;
      color: #b33f25;
    }

    &-description {
      text-align: center;
      font-family: "Roboto";
      font-weight: normal;
      font-size: 18px;
      color: #2b2b2b;
    }

    &-img {
      height: 85px;
    }
  }
}
</style>
