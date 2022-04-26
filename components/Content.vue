<template>
  <div class="intro">
    <div class="content-wrapper">
      <div class="sidebar">
        <div class="sidebar-content">
          <b>{{subline}}</b>
        </div>
      </div>
      <div class="content">
        <slot />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["subline"]
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
    margin-top: 2em;

    @include max-width($md) {
      flex-direction: column;
    }

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

      @include max-width($md) {
        transform: translate(0);
      }

      .sidebar-content {
        text-align: center;
        transform: translate(-50%) rotate(-90deg);
        white-space: nowrap;

        b {
          text-transform: uppercase;
          font-size: 0.8em;
        }

        @include max-width($md) {
          transform: translate(0%) rotate(0deg);
        }
      }
    }
    .content {
      flex: 4;
      max-width: 40em;
      h2 {
        @include max-width($md) {
          font-size: 2.5em;
        }
        @include max-width($sm) {
          font-size: 2em;
        }
      }
      p {
        text-align: justify;
        @include max-width($sm) {
          font-size: 0.9em;
        }
      }
    }
  }
}
</style>
