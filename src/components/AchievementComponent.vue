<template>
  <div class="achievement">
    <h3>{{ achievement.title }}</h3>
    <p>{{ achievement.description }}</p>
    <p>Points: {{ achievement.points }}</p>
  </div>
</template>

<script>
export default {
  props: {
    achievement: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
.achievement {
  margin-bottom: 20px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}
</style>
