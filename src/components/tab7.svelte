<script>
  import Carouselle_friuge_1 from "../components/carouselle_friuge_1.svelte";
  import Carouselle_friuge_2 from "../components/carouselle_friuge_2.svelte";
  import Carouselle_friuge_3 from "../components/carouselle_friuge_3.svelte";
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
    <br />
    <hr />
  </section>

  <!-- SECTION 2 -->
  <section class="max-w-[1100px] px-4">
    <div class="">
      <p class="preh2">FRIUGE 1</p>
      <h3 class="display">MALDIVERNE</h3>
      <Carouselle_friuge_1 />
    </div>
  </section>

  <!-- SECTION 3 -->
  <section class="max-w-[1100px] px-4">
    <div class="">
      <p class="preh2">FRIUGE 2</p>
      <h3 class="display">SRI LANKA</h3>
      <Carouselle_friuge_2 />
    </div>
  </section>

  <!-- SECTION 4 -->
  <section class="max-w-[1100px] px-4">
    <div class="">
      <p class="preh2">FRIUGE 3</p>
      <h3 class="display">THAILAND</h3>
      <Carouselle_friuge_3 />
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
    background-position-x: 30%;
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
