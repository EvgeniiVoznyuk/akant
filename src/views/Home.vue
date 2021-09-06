<template>
  <div class="home">
    <!-- <LearningWays /> -->
    <HowLearn />
    <OurTeachers />
    <Comments />
  </div>
</template>

<script>
/* eslint-disable vue/no-unused-components */
import LearningWays from "../components/LearningWays.vue";
import HowLearn from "../components/HowLearn.vue";
import Comments from "../components/Comments.vue";
import OurTeachers from "../components/OurTeachers.vue";

export default {
  name: "Home",
  components: {
    LearningWays,
    HowLearn,
    Comments,
    OurTeachers,
  },
};
</script>

<style lang="scss">
.home {
  width: 100%;
}
</style>
