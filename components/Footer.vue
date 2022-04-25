<template>
  <footer>
    <div class="footer-elements">
      <div class="footer-line">
        <div class="impressum-blocks">
          <div>
            <p>
            zynd GmbH<br/>
            Hofgasse 22<br/>
            4020 Linz, Austria
            </p>
          </div>
          <div>
            <p>
            Christoph Döberl<br/>
            office@zynd.at<br/>
            +43 676 7823454
            </p>
          </div>
          <div>
            <p>
            IBAN: AT19 3400 0000 0390 5437<br/>
            Firmenbuch: FN 575396 x<br/>
            UID: ATU77825016
            </p>
          </div>
        </div>
        <div class="logo">
          <svg viewBox="0 0 119.063 119.063" xmlns="http://www.w3.org/2000/svg"><path style="fill:#F0EDF4" d="M112.086 74.973v10.329H91.772v27.2h27.2v-37.53ZM.09 85.32v6.869h13.996L.09 105.686v6.834h25.07v-7.236H10.768l14.377-14.172V85.32zm27.19 0 13.242 25.107-3.608 8.635h7.717l.195-.45 3.565-8.59L58.754 85.32h-7.722l-6.946 16.558-8.751-16.558Zm33.671 0v27.2h7.231V92.206h13.084v20.314h6.886v-27.2Zm38.051 6.868h13.084v13.084H99.002Z"/><path style="fill:#9A37F8" d="M39.22 0 25.762 23.343l46.05-11.984 2.952-.769 2.773 10.619-17.95 23.486 40.03-10.417L79.854 0Zm20.21 25.8L19.444 36.18 39.22 70.472h40.634L93.33 47.102 62.875 55.03l-15.613 4.065-2.99.778-2.182-8.342-.589-2.282z"/></svg>
        </div>
      </div>
      <div class="footer-line">
        <NuxtLink to="/impressum">Impressum</NuxtLink>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
footer {
  min-height: 30vh;
  background: $color-dark;
  color: $color-light;

  .footer-elements {
    @include page-item;
    padding-top: 2em;

    display: flex;
    flex-direction: column;

    .footer-line {
      display: flex;
      flex-direction: row;

      > * {
        margin: 0 0 2em 0;
      }

      @include max-width($md) {
        flex-direction: column;
        align-items: center;
      }

      .impressum-blocks {
        > div {
          font-size: 0.8em;
          margin: 0 3em 0 0;
        }

        flex-grow: 1;
        display: flex;
        flex-direction: row;
        justify-content: flex-start;

        @include max-width($sm) {
          flex-direction: column;
          justify-content: space-between;
        }
      }

      .logo {
        width: 100px;
      }

      a {
        font-size: 0.8em;
        color: $color-light;
        text-decoration: none;
        &:hover {
          color: $color-primary;
        }
      }
    }
  }
}
</style>
