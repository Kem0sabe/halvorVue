<template>
  <div>
    <NavBar />

    <div id="introduction" class="space home-section">
      <IntroductionComponent />
    </div>
    <div id="achievements" class="space achievements-section">
      <AchievementsComponent />
    </div>
    <div id="form" class="space form-section">
      <FormComponent />
    </div>
  </div>
</template>

<script>
import NavBar from './NavBar.vue';
import IntroductionComponent from './IntroductionComponent.vue';
import AchievementsComponent from './AchievementsComponent.vue';
import FormComponent from './FormComponent.vue';

export default {
  name: 'HelloWorld',
  components: {
    NavBar,
    IntroductionComponent,
    AchievementsComponent,
    FormComponent
  },
  props: {
    msg: String
  }
}
</script>

<style scoped lang="scss">
  .space {
    margin-top: 100px;
  }
</style>
