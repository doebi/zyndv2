<template>
  <div class="highlight">
  </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
.highlight {
  min-height: 30vh;

  background-size: 600% 600%;
  animation: pulse 30s ease-in-out infinite;
  /*background: linear-gradient(120deg, $color-primary, $color-secondary, $color-tertiary);*/
  background: linear-gradient(-120deg, lighten($color-primary, 5%), darken($color-primary, 20%));
}
</style>
