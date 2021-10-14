<template>
  <div class="lw">
    <div class="lw__container container">
      <SectionTitle :title="'Направления обучения'" />
      <div class="lw__grid">
        <div class="way">
          <h1 class="way__title">Дизайн интерьера жилых помещений</h1>
          <p class="way__description">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Possimus
            aliquid eligendi minima ab voluptatem? Consectetur, dicta adipisci.
            Ullam praesentium doloribus dolorem error velit voluptatum provident
            suscipit, maxime, perferendis distinctio cupiditate?
          </p>
          <p class="way__date">Начало 6 июля</p>
          <a class="way__link">Подробнее</a>
        </div>

        <div class="way">
          <h1 class="way__title">Индивидуальное занятие</h1>
          <p class="way__description">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Possimus
            aliquid eligendi minima ab voluptatem? Consectetur, dicta adipisci.
            Ullam praesentium doloribus dolorem error velit voluptatum provident
            suscipit, maxime, perferendis distinctio cupiditate?
          </p>
          <p class="way__date">Начало 6 июля</p>
          <a class="way__link">Подробнее</a>
        </div>

        <div class="way">
          <h1 class="way__title">Программа ArchiCAD</h1>
          <p class="way__description">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Possimus
            aliquid eligendi minima ab voluptatem? Consectetur, dicta adipisci.
            Ullam praesentium doloribus dolorem error velit voluptatum provident
            suscipit, maxime, perferendis distinctio cupiditate?
          </p>
          <p class="way__date">Начало 6 июля</p>
          <a class="way__link">Подробнее</a>
        </div>

         <div class="way">
          <h1 class="way__title">Скетч для ландшафтных дизайнеров</h1>
          <p class="way__description">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Possimus
            aliquid eligendi minima ab voluptatem? Consectetur, dicta adipisci.
            Ullam praesentium doloribus dolorem error velit voluptatum provident
            suscipit, maxime, perferendis distinctio cupiditate?
          </p>
          <p class="way__date">Начало 6 июля</p>
          <a class="way__link">Подробнее</a>
        </div>

         <div class="way">
          <h1 class="way__title">Рисование с нуля</h1>
          <p class="way__description">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Possimus
            aliquid eligendi minima ab voluptatem? Consectetur, dicta adipisci.
            Ullam praesentium doloribus dolorem error velit voluptatum provident
            suscipit, maxime, perferendis distinctio cupiditate?
          </p>
          <p class="way__date">Начало 6 июля</p>
          <a class="way__link">Подробнее</a>
        </div>

         <div class="way">
          <h1 class="way__title">Скетч в интерьере</h1>
          <p class="way__description">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Possimus
            aliquid eligendi minima ab voluptatem? Consectetur, dicta adipisci.
            Ullam praesentium doloribus dolorem error velit voluptatum provident
            suscipit, maxime, perferendis distinctio cupiditate?
          </p>
          <p class="way__date">Начало 6 июля</p>
          <a class="way__link">Подробнее</a>
        </div>
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
.way {
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 30px;
  width: 360px;
  height: 360px;
  border-radius: 50%;
  padding: 20px;

  background-color: #f3f2f2;

  font-family: "Montserrat";

  &__title {
    padding-top: 60px;
    font-size: 20px;
    color: #D04D30;
  }

  &__description {
    color: rgba(24, 24, 24, 0.87);
    line-height: 18px;
  }

  &__link {
    font-weight: bold;
    color: #D04D30;
    cursor: pointer;
  }
}
.lw {
  display: flex;
  justify-content: center;
  background-image: url("~@/assets/img/waysBg.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  padding-bottom: 100px;

  &__grid {
    display: grid;
    gap: 20px;
    grid-template-columns: repeat(3, 1fr);

    @media screen and (max-width: 1280px) {
      grid-template-columns: repeat(2, 1fr);
      gap: 40px;
    }

    @media screen and (max-width: 865px) {
      grid-template-columns: repeat(1, 1fr);
      gap: 40px;
    }
  }

  &__container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 100px;
    padding-top: 50px;
  }
}
</style>
