<template>
  <div class="comments">
    <div class="comments__container container">
      <SectionTitle :title="'Отзывы'" />

      <div class="comments__group">
        <div class="comment">
          <img src="~@/assets/img/comment/img1.jpeg" class="comment__img" />
          <p class="comment__name">Татьяна Гайдукова</p>
          <p class="comment__description">
            Очень благодарна Виталию за качественную и интересную информацию.
            Это тот самый случай, когда преподаватель искренне любит свою
            профессию и это видно по тому, как он ведёт уроки. Увлечённость
            предметом передается слушателям, благодаря чему на лекциях царит
            творческая атмосфера. Восхищаюсь всеми талантами Виталия!
          </p>
          <div class="comment__icons">
            <img src="~@/assets/img/comment/inst.svg" class="comment__icon" />
            <img src="~@/assets/img/comment/msg.svg" class="comment__icon" />
          </div>
        </div>
        <div class="comment">
          <img src="~@/assets/img/comment/img2.jpeg" class="comment__img" />
          <p class="comment__name">Людмила Гайдученко</p>
          <p class="comment__description">
            Огромная благодарность Виталию! Отличный педагог, легко и доступно
            излагает материал, находит подход ко всем. Благодарна Виталию за то,
            что вселил уверенность в себе. Для меня, как для человека который
            никогда не ходил в художественную школу, а просто рисовал потому что
            нравится, это очень важно. Даже после одного занятия хочется
            рисовать, рисовать и ещё раз рисовать
          </p>
          <div class="comment__icons">
            <img src="~@/assets/img/comment/inst.svg" class="comment__icon" />
            <img src="~@/assets/img/comment/msg.svg" class="comment__icon" />
          </div>
        </div>
        <div class="comment">
          <img src="~@/assets/img/comment/img.png" class="comment__img" />
          <p class="comment__name">Андрей Молодоженя</p>
          <p class="comment__description">
            Очень рекомендую занятия по дизайну у Виталия! У Виталия есть все,
            что необходимо: профессиональное образование по архитектуре, большой
            разноплановый практический опыт по дизайну и проектированию, редкий
            талант интересно и качественно делиться информацией с учениками.
          </p>
          <div class="comment__icons">
            <img src="~@/assets/img/comment/inst.svg" class="comment__icon" />
            <img src="~@/assets/img/comment/msg.svg" class="comment__icon" />
          </div>
        </div>
      </div>

      <button class="btn">Начать обучение с нами</button>

      <div class="comments__akant-school akant-school">
        <img src="~@/assets/img/bigCol.png" class="akant-school__img" />
        <div class="akant-school__title-group">
          <h1 class="akant-school__title">Школа дизайна и творчества</h1>
          <img src="~@/assets/img/akantH.svg" class="akant-school__img-logo" />
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
.comment {
  width: 320px;
  border: 1px solid #00000044;
  padding: 40px;

  display: flex;
  flex-direction: column;
  align-items: start;
  gap: 20px;

  font-family: "Montserrat";
  font-weight: normal;
  color: #000;

  &__name {
    font-size: 16px;
  }

  &__description {
    line-height: 1.2;
  }

  &__icons {
    display: flex;
    gap: 10px;
  }

  &__icon {
    cursor: pointer;
  }

  &__img {
    width: 90px;
    height: 90px;
    border-radius: 50%;
  }
}
.comments {
  display: flex;
  justify-content: center;
  background-image: url("~@/assets/img/bg.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  height: 1200px;
  padding-bottom: 50px;

  &__group {
    display: flex;
    gap: 30px;
  }

  &__container {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    padding-top: 50px;
  }
}
.akant-school {
  justify-self: end;
  display: flex;
  gap: 50px;

  &__title {
    font-family: "Roboto";
    font-size: 56px;
    font-weight: 400;
    padding-bottom: 10px;
  }

  &__img {
    &-logo {
      padding-left: 140px;
    }
  }
}
</style>
