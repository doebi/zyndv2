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
  background: linear-gradient(120deg, rgba(154,55,248,1), rgba(49,40,125,1), rgba(67,168,244,1));
}
</style>
