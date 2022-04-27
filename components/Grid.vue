<template>
  <div class="grid">
    <div class="content-wrapper">
      <slot />
    </div>
  </div>
</template>

<script>
export default {
  props: ["subline"]
}
</script>

<style lang="scss" scoped>
.grid {
  min-height: 30vh;
  margin-bottom: 7em;

  .content-wrapper {
    @include page-item;
    display: flex;
    justify-content: center;
    margin-top: 2em;

    @include max-width($md) {
      flex-direction: column;
    }
  }
}
</style>
