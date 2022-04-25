<template>
  <header>
    <div class="header-elements">
      <div class="menu">
        <div class="menu-entry">
          <NuxtLink to="/about">About Us</NuxtLink>
        </div>
        <div class="menu-entry">
          <NuxtLink nuxt to="/services">Services</NuxtLink>
        </div>
        <div class="menu-entry">
          <NuxtLink nuxt to="/projects">Projects</NuxtLink>
        </div>
      </div>
      <div class="logo-pictogram">
        <NuxtLink nuxt to="/">
        <svg viewBox="0 0 119.062 104.775" xmlns="http://www.w3.org/2000/svg"><path d="M29.351.059 9.336 34.767l45.23-11.774 23.185-6.036 4.442-1.156 3.239 12.388.874 3.389L59.683 66.4l59.38-15.413L89.694.058ZM59.448 38.34 0 53.81l29.351 50.906h60.343l19.987-34.666-68.387 17.797-4.385 1.142-4.119-15.77Z"/></svg>
        </NuxtLink>
      </div>
      <div class="logo-text">
        <NuxtLink nuxt to="/">
        <svg viewBox="0 0 119.063 44.185" xmlns="http://www.w3.org/2000/svg"><path d="M112.166 0v10.344H91.82v27.242h27.243V0ZM0 10.363v6.878h14.016L0 30.76v6.846h25.108v-7.25H10.694l14.399-14.192v-5.8zm27.232 0 13.26 25.145-3.613 8.649h7.73l.195-.452 3.57-8.603 10.379-24.74h-7.734l-6.956 16.584-8.765-16.583Zm33.722 0v27.242h7.241V17.259H81.3v20.346h6.896V10.363Zm38.108 6.878h13.104v13.104H99.062Z"/></svg>
        </NuxtLink>
      </div>
    </div>
  </header>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
header {
  z-index: 999;
  top: 0;
  position: sticky;
  background-color: rgba($color-light, 0.75);
  backdrop-filter: blur(12px);

  .header-elements {
    @include page-item;
    padding: 2em 0.5em;

    display: flex;
    justify-content: flex-end;
    > div {
      height: 3em;
    }

    .logo-pictogram {
      svg {
        height: 100%;
        fill: $color-primary;
      }
    }
    .logo-text {
      overflow: hidden;
      display: flex;
      align-items: center;
      > a {
        display: flex;
        align-items: center;
      }

      &.animated {
        max-width: 0;
        opacity: 0;
        transition: max-width 1s, opacity 0.5s;
      }

      svg {
        height: 2em;
        padding-left: 10px;
        fill: $color-dark;
      }
    }
    &:hover {
      .logo-text {
        max-width: 150px;
        opacity: 1;
      }
    }

    .menu {
      flex: 1;
      display: flex;

      .menu-entry {
        display: flex;
        flex-direction: column;
        justify-content: center;
        white-space: nowrap;

        margin-right: 1em;
        cursor: pointer;

        a {
          transition: color 0.1s;
          color: $color-dark;
          text-decoration: none;
          &:hover {
            color: $color-primary;
          }
        }
      }
    }
  }
}
</style>
