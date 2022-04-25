<template>
  <div class="intro">
    <div class="content-wrapper">
      <div class="sidebar">
        <div class="sidebar-content">
          <b>Digitization: </b><span>The good, the bad the ugly.</span>
        </div>
      </div>
      <div class="content">
        <h2>Welcome to a new world of digital solutions and technology.</h2>
        <h4>Strategy & Business Innovation for your Company</h4>
        <p>Vel numquam molestiae necessitatibus dolorem molestiae nulla atque. Tempore et
voluptas non. Quis dolores placeat aut earum et vel.
Odio aut voluptas nihil mollitia nemo natus necessitatibus aperiam. Eveniet dolore
voluptatibus blanditiis et hic. Necessitatibus eum autem esse velit sed deserunt eum
labore. Corrupti et ratione quis laudantium architecto. Accusantium eos explicabo
laudantium ut repudiandae quam velit eoso. Ut earum aperiam distinctio quo.</p>
        <p>Facilis optio delectus ex. Qui perferendis quasi quis. Voluptatem optio doloremque
voluptas sed eum. Ut animi laborum adipisci perspiciatis tempore voluptas ut et.
Ut sequi velit architecto soluta voluptatum. Eum a ut repudiandae quis dolores
laudantium, occaecati incidunt nobis explicabo nam est. Ceaturerum fuga. Unti ommo
tore, sim nonsequi sume volore conseque volectem qui. Ut molupic atioratet eniminctae
nihicitatum remolor aut lictore, corunda nonseque pa plibea cus maio officident eos
diti ne arciducius saperum que dolorestia aspiet</p>
        <p>Officit acepel molupta venditiumet officil illecust, nonsequi consequam eos denis
nihiciis eicatem aborum lit aut in rerit, quiscip icimoloreri a vero es nos volorit, quisqui
busaectamus, audiore pelest, odia dolum volest eratur, ut modit, omnis et quo consendae
modia non peritio rentis nihit quid eum que rest, intiusc ipsanihilla vel ellaccum quassec.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="scss">
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
