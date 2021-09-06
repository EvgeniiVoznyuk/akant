<template>
  <div class="ot">
    <div class="ot__container container">
      <SectionTitle :title="'Наши преподаватели'" />

      <div class="ot__teachers">
        <div class="ot__row">
          <div class="ot__description description description--1">
            <p class="description__name">Name Surname</p>
            <p class="description__status">Основатель студии АКАНТ</p>
            <p class="description__text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae
              inventore suscipit, eligendi soluta ab similique, nam quia totam
              voluptates alias itaque corrupti consequuntur est rem quas omnis
              sed quis repudiandae. corrupti consequuntur est rem quas omnis
              sed quis repudiandae.
            </p>
            <a href="#" class="description__more">Больше |</a>
          </div>
          <img src="~@/assets/img/teachers/1.png" class="description__img">
        </div>

        <div class="ot__row ot__row--1">
          <img src="~@/assets/img/teachers/2.png" class="description__img">

          <div class="ot__description description description--2">
            <p class="description__name">Name Surname</p>
            <p class="description__status">Основатель студии АКАНТ</p>
            <p class="description__text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae
              inventore suscipit, eligendi soluta ab similique, nam quia totam
              voluptates alias itaque corrupti consequuntur est rem quas omnis
              sed quis repudiandae. corrupti consequuntur est rem quas omnis
              sed quis repudiandae.
            </p>
            <a href="#" class="description__more">Больше |</a>
          </div>
        </div>
      </div>

      <SectionTitle :title="'Примеры работ'" />
      <div class="examples">
        <img src="~@/assets/img/examples.jpeg" class="examples__img">
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
  width: 615px;
  height: 467px;
  padding: 40px;

  display: flex;
  flex-direction: column;
  gap: 30px;

  position: relative;

  &--1 {
    bottom: 5px;
    left: 10px;
  }

  &--2 {
    bottom: 5px;
    right: 39px;
  }

  font-family: "Montserrat";

  &__more {
    position: absolute;
    bottom: 40px;
    right: 40px;
    text-decoration: none;
    color: #b33f25;
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
    line-height: 24px;
  }
}

.ot {
  display: flex;
  justify-content: center;
  background-image: url("~@/assets/img/bg.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  // height: 1500px;
  padding-bottom: 50px;

  &__row {
    display: flex;
    align-items: center;

    position: relative;

    &--1 {
      bottom: 20px;
    }
  }

  &__container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 80px;
    padding-top: 50px;
  }
}
</style>
