<script>
  import Carouselle_aktiv from "../components/carouselle_aktiv.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section>
    <h2>ADVENTURE, OPLEVELSER & AKTIVITETER</h2>
    <p>
      I løbet af dit ophold hos os, er det muligt at deltage i vores
      spændingsfyldte udflugter og dagsture. Besøg vandfald, tag på
      snorkeleventyr og tag på en ATV-køretur, hvor du kan udforske junglen og
      de øde strande.
    </p>
  </section>

  <p class="preh2">TILFØJELSER & AKTIVITETER</p>
  <h3 class="">Tilføj endnu mere god stemning</h3>

  <!-- SECTION 2 -->
  <section class="">
    <div class="">
      <p class="preh2 text-center">AKTIVITET I OMRÅDET</p>
      <h3 class="display text-center">SRI LANKA</h3>
      <p class="text-center">Uendelige oplevelser og muligheder</p>
      <Carouselle_aktiv />
    </div>
  </section>

  <!-- SECTION 3 -->
  <section class="">
    <div class="">
      <p class="preh2 text-center">SKRI LANKA</p>
      <h3 class="display text-center">FRIUGE 2</h3>
      <p class="text-center">Adventure & aktion</p>
      <Carouselle_aktiv />
    </div>
  </section>

  <!-- SECTION 4 -->
  <section class="">
    <div class="">
      <p class="preh2 text-center">HAWAII</p>
      <h3 class="display text-center">FRIUGE 3</h3>
      <p class="text-center">Afslapning, shopping og surfing</p>
      <Carouselle_aktiv />
    </div>
  </section>
</main>

<style>
  .display {
    font-family: var(--h2_text);
    font-size: var(--font_h2);
    color: var(--sort);
    line-height: var(--line-m);
    padding: var(--spacing-10);
  }
</style>
