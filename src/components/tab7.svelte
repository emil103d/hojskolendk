<script>
  import Carouselle_friuge_1 from "../components/carouselle_friuge_1.svelte";
  import Carouselle_friuge_2 from "../components/carouselle_friuge_2.svelte";
  import Carouselle_friuge_3 from "../components/carouselle_friuge_3.svelte";
  import MyButton from "../components/button.svelte";
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

  <section class="flex justify-end px-4">
    <MyButton type="linkbutton">
      ADVENTURE<svg
        class="m-auto"
        width="18"
        height="16"
        viewBox="0 0 18 16"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M17.7071 8.70711C18.0976 8.31658 18.0976 7.68342 17.7071 7.29289L11.3431 0.928932C10.9526 0.538408 10.3195 0.538408 9.92893 0.928932C9.53841 1.31946 9.53841 1.95262 9.92893 2.34315L15.5858 8L9.92893 13.6569C9.53841 14.0474 9.53841 14.6805 9.92893 15.0711C10.3195 15.4616 10.9526 15.4616 11.3431 15.0711L17.7071 8.70711ZM17 7L-4.76837e-07 7V9L17 9V7Z"
          fill="#929292"
        />
      </svg>
    </MyButton>
  </section>
</main>

<style>
  main {
    background-image: url(../../gurfers.png);
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
