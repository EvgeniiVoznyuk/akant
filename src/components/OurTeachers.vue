<template>
  <div class="ot">
    <div class="ot__container container">
      <SectionTitle :title="'Наши преподаватели'" />

      <div class="ot__teachers">
        <div class="ot__row">
          <div class="ot__description description description--1">
            <p class="description__name">Виталий Дриженко</p>
            <p class="description__status">Основатель студии АКАНТ</p>
            <p class="description__text">
              Практикующий архитектор, дизайнер интерьера, с опытом
              проектирования жилых и коммерческих объектов более 18 лет. Автор
              программ обучения - "Дизайн интерьера жилых помещений",
              "ArchiCad", "СКЕТЧ ".
            </p>
            <a href="#" class="description__more">Больше |</a>
          </div>
          <div class="description__img description__img--2" />
        </div>

        <div class="ot__row ot__row--1">
          <div class="description__img description__img--1" />

          <div class="ot__description description description--2">
            <p class="description__name">Наталья Лысенко</p>
            <p class="description__status">Основатель студии АКАНТ</p>
            <p class="description__text">
              Основатель студии дизайна "DARTS comfort", дизайнер интерьера,
              визуализатор, автор программы обучения " Преимущества Sketchup для
              дизайнеров интерьера"
            </p>
            <a href="#" class="description__more">Больше |</a>
          </div>
        </div>
      </div>

      <SectionTitle :title="'Примеры работ'" />
      <div class="examples">
        <img src="~@/assets/img/examples.jpeg" class="examples__img" />
      </div>
    </div>
  </div>
</template>

<script>
import SectionTitle from "./SectionTitle.vue";
export default {
  components: {
    SectionTitle,
  },
};
</script>

<style lang="scss">
.description {
  box-sizing: border-box;
  background-color: #f5f4f4;
  width: 515px;
  height: 750px;
  padding: 40px;

  display: flex;
  flex-direction: column;
  gap: 30px;

  position: relative;

  &__img {
    width: 515px;
    height: 750px;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;

    &--1 {
      background-image: url("~@/assets/img/ms.jpeg");
    }

    &--2 {
      background-image: url("~@/assets/img/mr.jpeg");
    }
  }

  font-family: "Montserrat";

  &__more {
    position: absolute;
    bottom: 40px;
    right: 40px;
    text-decoration: none;
    color: #b33f25;
  }

  &__status {
    font-size: 18px;
  }

  &__name {
    color: #b33f25;
    font-size: 24px;
    line-height: 29px;
    font-weight: 900;
  }

  &__text {
    font-weight: normal;
    max-width: 420px;
    line-height: 30px;
    font-size: 20px;
  }
}

.ot {
  display: flex;
  justify-content: center;
  background-image: url("~@/assets/img/bg.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  padding-bottom: 50px;

  &__row {
    display: flex;
    align-items: center;

    gap: 30px;
  }

  &__container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 80px;
    padding-top: 50px;
  }

  &__teachers {
    display: flex;
    flex-direction: column;
    gap: 30px;
  }
}
</style>
