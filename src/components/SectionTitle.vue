<template>
  <div class="col">
    <img src="~@/assets/img/col.png" class="col__img" />
    <div class="col__line" />
    <span class="montserrat col__title">{{ title }}</span>
    <div class="col__line" />
    <img src="~@/assets/img/col.png" class="col__img" />
  </div>
</template>

<script>
export default {
  name: "SectionTitle",
  props: {
    title: {
      type: String,
    },
  },

}
</script>

<style lang="scss" scoped>
.col {
  width: 90%;
  display: flex;
  align-items: center;
  justify-content: space-between;

  &__line {
    width: 130px;
    height: 1px;
    background-color: #000;

     @media screen and (max-width: 1180px) {
      & {
        width: 70px;
      }
    }
  }

  &__title {
    font-size: 36px;
    color: #B33F25;

    @media screen and (max-width: 1180px) {
      & {
        font-size: 26px;
      }
    }
  }

   @media screen and (max-width: 1180px) {
      &__img {
        width: 70px;
      }
    }
}
</style>
