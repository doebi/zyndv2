<template>
  <div class="intro">
    <div class="content-wrapper">
      <div class="sidebar">
        <div class="sidebar-content">
          <b>Who we are</b>
        </div>
      </div>
      <div class="content">
        <h2>About Us</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
.intro {
  min-height: 30vh;
  margin-bottom: 7em;

  .content-wrapper {
    @include page-item;
    display: flex;
    justify-content: flex-end;

    .sidebar {
      user-select: none;
      z-index: -1;
      flex: 1;
      max-width: 10em;
      color: $color-primary;
      display: flex;
      flex-direction: row;
      align-items: center;
      transform: translate(50%);

      .sidebar-content {
        text-align: center;
        transform: translate(-50%) rotate(-90deg);
        white-space: nowrap;
      }
    }
    .content {
      flex: 4;
      max-width: 40em;
      p {
        text-align: justify;
      }
    }
  }
}
</style>
