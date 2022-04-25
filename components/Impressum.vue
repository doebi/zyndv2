<template>
  <div class="intro">
    <div class="content-wrapper">
      <div class="sidebar">
        <div class="sidebar-content">
          <b>Impressum</b>
        </div>
      </div>
      <div class="content">
        <p>
        zynd GmbH<br>
        Unternehmensgegenstand:<br>
        Dienstleistungen in der automatischen Datenverarbeitung und Informationstechnik<br>
        </p>

        <p>
        Gewerbeordnung: www.ris.bka.gv.at<br>
        Mitglied der WKÖ, WKOÖ<br>
        </p>

        <p>
        UID-Nr: ATU77825016<br>
        FN: 575396x<br>
        FB-Gericht: Landesgericht Linz<br>
        </p>

        <p>
        Hofgasse 22<br>
        4020 Linz<br>
        Österreich<br>
        </p>

        <p>
        +43 676 7823454<br>
        office@zynd.at<br>
        </p>
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
