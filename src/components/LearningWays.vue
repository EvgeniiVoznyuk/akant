<template>
  <div class="lw">
    <div class="lw__container container">
      <SectionTitle :title="'Направления обучения'" />
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
.lw {
  display: flex;
  justify-content: center;
  background-image: url("~@/assets/img/waysBg.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  height: 1200px;

  &__container {
    display: flex;
    align-items: flex-start;
    padding-top: 50px;
  }
}
</style>
