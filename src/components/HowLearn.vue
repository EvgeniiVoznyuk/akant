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
            ОНЛАЙ-школа дизайна «АКАНТ» создала собственное творческое
            онлайн-пространство, в котором главным критерием успешного обучения
            стала атмосфера творческой мастерской. Это создает оптимальные
            условия для процесса обучения и творческого вдохновения.
          </p>
        </div>

        <div class="grid__item">
          <img
            src="~@/assets/img/gridImages/clock.svg"
            class="grid__item-img"
          />
          <h1 class="grid__item-title">Комфортный темп обучение</h1>
          <p class="grid__item-description">
            Формат ОНЛАЙН-обучения позволит выбрать удобное время для вашего
            обучения. Занятия представляют собой живое общение, в котором
            учитывается индивидуальные особенности каждого ученика.
          </p>
        </div>

        <div class="grid__item">
          <img
            src="~@/assets/img/gridImages/support.svg"
            class="grid__item-img"
          />
          <h1 class="grid__item-title">Постоянная поддержка куратора</h1>
          <p class="grid__item-description">
            Одним из важнейших преимуществ нашей ОНЛАЙН-школы является
            индивидуальное обучение. Программа обучения, в этом случае,
            разрабатывается с учетом конкретики ваших задач, пожеланий,
            предшествующего опыта и специфики практического применения
          </p>
        </div>

        <div class="grid__item">
          <img src="~@/assets/img/gridImages/hts.svg" class="grid__item-img" />
          <h1 class="grid__item-title">Разбор домашних заданий</h1>
          <p class="grid__item-description">
            В ОНЛАЙН-формате практическая работа и консультации по проекту более
            эффективна, чем на обычных занятиях. Отвечая на вопросы слушателя,
            преподаватель может использовать свой весь архивный материал,
            проекты, чертежи, визуализацию, а также использовать для наглядности
            сразу несколько программ.
          </p>
        </div>

        <div class="grid__item">
          <img
            src="~@/assets/img/gridImages/clock.svg"
            class="grid__item-img"
          />
          <h1 class="grid__item-title">Практики</h1>
          <p class="grid__item-description">
            Обучение дизайну интерьера ведется по авторской программе,
            разработанной преподавательским составом из практикующих
            архитекторов, дизайнеров интерьеров, художников и других
            специалистов разного профиля. В нашей мастерской вы сможете изучить
            базовую теорию и закрепить ее на практических занятиях.
          </p>
        </div>

        <div class="grid__item">
          <img
            src="~@/assets/img/gridImages/diploma.svg"
            class="grid__item-img"
          />
          <h1 class="grid__item-title">Диплом после окончания</h1>
          <p class="grid__item-description">
            После обучения Вы защищаете дипломную работу, в которой
            продемонстрируете созданный вами дизайн проект с технической
            документацией и трехмерной визуализацией, которая станет первой в
            вашем портфолио и получаете Сертификат. И только у нас Вы получите
            поддержку кураторов курса на протяжении вашего первого проекта
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
              Научим мыслить и творить как дизайнер, автоматизировать и
              грамотно оформлять проектную документацию. В нашей школе особое
              внимание уделяется техническим вопросам, с которыми сталкиваются
              начинающие и практикующие дизайнеры.
            </p>
          </div>
          <div class="atmosphere__imgs">
            <img
              src="~@/assets/img/atmosphere/1.png"
              class="atmosphere__img atmosphere__img--1"
            />
            <div class="atmosphere__img-groups">
              <div class="atmosphere__imgs-group atmosphere__imgs-group--1">
                <img
                  src="~@/assets/img/atmosphere/2.png"
                  class="atmosphere__img atmosphere__img--2"
                />
                <img
                  src="~@/assets/img/atmosphere/3.png"
                  class="atmosphere__img atmosphere__img--2"
                />
              </div>
              <div class="atmosphere__imgs-group atmosphere__imgs-group--2">
                <img
                  src="~@/assets/img/atmosphere/4.png"
                  class="atmosphere__img atmosphere__img--2"
                />
                <img
                  src="~@/assets/img/atmosphere/5.png"
                  class="atmosphere__img atmosphere__img--2"
                />
              </div>
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

  &__img-groups {
    display: flex;
    gap: 20px;
  }

  &__imgs {
    display: flex;
    justify-content: center;
    gap: 20px;

    &-group {
      width: 300px;

      &--1 {
        padding-top: 70px;
      }
      &--2 {
        padding-top: 110px;
      }
    }
  }

  &__img {
    &--1 {
      width: 600px;
      height: 650px;
    }
  }

  @media screen and (max-width: 1310px) {
    &__imgs {
      gap: 10px;

      &-group {
        width: 270px;
      }
    }

    &__img {
      &--1 {
        width: 500px;
        height: 550px;
      }

      &--2 {
        width: 268px;
        height: 224px;
      }
    }

    &__title {
      width: 400px;
    }
  }

  @media screen and (max-width: 1060px) {
    &__description {
      position: relative;
      top: 110px;
      padding-left: 20px;
      width: 400px;
    }

    &__img-groups {
      display: none;
    }

    &__imgs {
      justify-content: flex-start;
    }

    &__text-group {
      display: flex;
      gap: 60px;
      position: relative;
      top: 40px;
    }
  }

  @media screen and (max-width: 960px) {
    & {
      display: none;
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
    width: 360px;
    display: flex;
    gap: 20px;
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
      font-size: 16px;
      color: #2b2b2b;
      line-height: 22px;
    }

    &-img {
      height: 85px;
    }
  }

  @media screen and (max-width: 1280px) and (min-width: 1040px) {
    &__item {
      width: 280px;

      &-title {
        font-size: 16px;
      }
    }
  }

  @media screen and (max-width: 1040px) {
    & {
      grid-template-columns: repeat(2, 1fr);
      gap: 100px;
    }
  }

  @media screen and (max-width: 850px) {
    & {
      grid-template-columns: repeat(1, 1fr);
    }
  }
}
</style>
