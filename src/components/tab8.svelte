<script>
  import Carouselle_aktiv from "../components/carouselle_aktiv.svelte";
</script>

<main class="col-start-2 w-[99%]">
  <!-- SECTION 1 -->
  <section class="maxwidthwrapper" id="no-pad">
    <h2>ADVENTURE, OPLEVELSER & AKTIVITETER</h2>
    <p>
      I løbet af dit ophold hos os, er det muligt at deltage i vores
      spændingsfyldte udflugter og dagsture. Besøg vandfald, tag på
      snorkeleventyr og tag på en ATV-køretur, hvor du kan udforske junglen og
      de øde strande.
    </p>
<<<<<<< HEAD
    <br />
    <hr class="py-5" />
=======
    <br>
    <hr>
>>>>>>> 20dd96638b8cfca2ac71296c218a5c1a74ceb0d6
  </section>

  <!-- SECTION 2 -->
  <section class="max-w-[1100px] px-4">
    <div class="">
      <p class="preh2">ADVENTURE & AKTIVITETER</p>
      <h3 class="display">MALDIVERNE</h3>
      <Carouselle_aktiv />
    </div>
  </section>

  <!-- SECTION 3 -->
  <section class="max-w-[1100px] px-4">
    <div class="">
      <p class="preh2">ADVENTURE & AKTIVITETER</p>
      <h3 class="display">SRI LANKA</h3>
      <Carouselle_aktiv />
    </div>
  </section>

  <!-- SECTION 4 -->
  <section class="max-w-[1100px] px-4">
    <div class="">
      <p class="preh2">ADVENTURE & AKTIVITETER</p>
      <h3 class="display">THAILAND</h3>
      <Carouselle_aktiv />
    </div>
  </section>
</main>

<style>
  main {
    background-image: url(src/_icons/gurfers.png);
    background-position: cover;
    background-size: 200%;
    background-repeat: repeat-y;
    background-position-y: 80%;
    background-position-x: 80%;
  }
  .display {
    font-family: var(--h2_text);
    font-size: var(--font_h2);
    color: var(--sort);
    line-height: var(--line-m);
  }

  #no-pad {
    padding-top: 0;
  }

  section {
    padding-top: var(--padding-sections);
    padding-bottom: var(--padding-sections);
  }
</style>
