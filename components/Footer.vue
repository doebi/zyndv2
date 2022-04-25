<template>
  <footer>
    <div class="footer-elements">
      <div>
        <p>
        zynd GmbH<br/>
        UID: ATU77825016
        </p>
      </div>
      <div>
        <p>
        Hofgasse 22<br/>
        4020 Linz, Austria
        </p>
      </div>
      <div>
        <p>
        IBAN: AT19 3400 0000 0390 5437<br/>
        Firmenbuch: FN 575396 x
        </p>
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
  min-height: 20vh;
  background: $color-dark;
  color: $color-light;

  .footer-elements {
    @include page-item;
    padding: 2em 0.5em;

    > div {
      font-size: 0.8em;
      margin: 0 1em;
    }

    display: flex;
    justify-content: start;
    flex-direction: row;
  }
}
</style>
