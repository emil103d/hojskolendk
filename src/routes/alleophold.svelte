<script>
  import { onMount } from "svelte"; //Filtrering skal vise sig når siden loader (lifecycle) når siden loader vil den automatisk kalde f.eks. getVarigheder
  import Header from "../components/header.svelte";
  import { opholdData } from "../stores/opholdData.js"; // Henter dataen ned
  import Menu from "../components/menu.svelte";
  import Afrejseselekt from "../components/afrejse.svelte";
  import Ophold from "../components/ophold.svelte";

  let varighed = []; // Tomt array til varighederne
  let afrejser = []; // Tomt array til afrejse
  let selectedvar = ""; //  menu selection
  let selectedAf = ""; //  menu selection

  const getVarigheder = () => {
    //Funktion der henter de forskellige varigheder
    for (let opholdObj of opholdData) {
      //Hvert ophold vil være opholdObj og opholdObj.varig henter værdien fra opholddata
      if (!varighed.includes(opholdObj.varig)) {
        // Kigger arrayet igennem og hvis den ikke har den værdi skal den tilføje værdien i arrayet
        varighed = [...varighed, opholdObj.varig]; //Tilføjer værdien hvis det ikke er der sammen med alle de andre værdier
      }
    }
    varighed = varighed.sort(); // efter den har hentet alle unikke værdierne ind i arrayet skal de sorteres
  };
  onMount(() => getVarigheder());

  const getAfrejser = () => {
    for (let opholdObj of opholdData) {
      if (!afrejser.includes(opholdObj.afrejse)) {
        afrejser = [...afrejser, opholdObj.afrejse];
      }
    }
    afrejser = afrejser.sort();
  };
  onMount(() => getAfrejser());

  // Query results
  let filteredOphold = [];

  // For Select Menu
  $: if (selectedvar) getOpholdByVar(); //Svelte reaktiv condition -> if selected varighed er sand kald funktion
  $: console.log(filteredOphold, selectedvar);

  $: if (selectedAf) getOpholdByAfrejse();
  $: console.log(filteredOphold, selectedAf);

  const getOpholdByVar = () => {
    if (selectedvar === "alle") {
      // Hvis der er blevet valgt se alle valgmuligheder knappen
      return (filteredOphold = []); // Er det ligmed et tomt array da den så vil kalde else sektion med alle opholdende
    }
    return (filteredOphold = opholdData.filter(
      (ophold) => ophold.varig === selectedvar // Filter ud de ophold der matcher den valgte varighed
    ));
  };

  const getOpholdByAfrejse = () => {
    if (selectedAf === "alle") {
      // Hvis der er blevet valgt se alle valgmuligheder knappen
      return (filteredOphold = []); // Er det ligmed et tomt array da den så vil kalde else sektion med alle opholdende
    }
    return (filteredOphold = opholdData.filter(
      (ophold) => ophold.afrejse === selectedAf // Filter ud de ophold der matcher den valgte varighed
    ));
  };
</script>

<img src="ferie9.webp" alt="herobillede" class="hero-image" />
<div class="hero-text">
  <p>HØJSKOLEOPHOLD FOR UNGE</p>
  <h1>LAD DIG INSPIRERE AF ALLE VORES SPÆNDENDE OPHOLDE</h1>
</div>

<main class="maxwidthwrapper">
  <div class="preh2">
    <a href="indec">Forside /</a>
    <a href="alleophold" class="underline preh2">Alle højskoleophold</a>
  </div>
  <!-- SECTION 1  -->
  <section class="" id="no-pad">
    <h2>Hvor drømmer du om at rejse hen?</h2>
    <p>
      Drømmer du om et friår fra studierne, en pause fra udannelsesræsset eller
      bare har lyst til et opleve verdenen? Så dyk ned og læs mere om vores
      spændende højskoleophold og tag med os ud og udfroske verdenen!
    </p>
    <br />
    <hr />
    <div class="flex justify-center gap-5 pt-20">
      <Menu {varighed} bind:selectedvar />
      <Afrejseselekt {afrejser} bind:selectedAf />
    </div>
  </section>

  <!-- SECTION 2 -->
  <section>
    <article id="alleophold" class="">
      {#if filteredOphold.length > 0}
        {#each filteredOphold as { title, image, subtitle, dato, afrejse, pris, undervisning, varig }}
          <Ophold
            {image}
            {title}
            {subtitle}
            {dato}
            {afrejse}
            {pris}
            {undervisning}
            {varig}
          />
        {/each}
      {:else}
        {#each opholdData as { title, image, subtitle, dato, afrejse, pris, undervisning, varig }}
          <Ophold
            {image}
            {title}
            {subtitle}
            {dato}
            {afrejse}
            {pris}
            {undervisning}
            {varig}
          />
        {/each}
      {/if}
    </article>
  </section>

  <!-- SECTION 3 -->
  <section>
    <article id="alleophold" class="">
      {#if filteredOphold.length > 0}
        {#each filteredOphold as { title, image, subtitle, dato, afrejse, pris, undervisning, varig }}
          <Ophold
            {image}
            {title}
            {subtitle}
            {dato}
            {afrejse}
            {pris}
            {undervisning}
            {varig}
          />
        {/each}
      {:else}
        {#each opholdData as { title, image, subtitle, dato, afrejse, pris, undervisning, varig }}
          <Ophold
            {image}
            {title}
            {subtitle}
            {dato}
            {afrejse}
            {pris}
            {undervisning}
            {varig}
          />
        {/each}
      {/if}
    </article>
  </section>
</main>

<!-- Hvis filtreret ophold har ophold i sig hvis de filtreret ophold go ellers hvis alle ophold  -->

<!-- <main id="alleophold" class="w-full grid justify-center maxwidthwrapper">
  {#if filteredOphold.length > 0}
    {#each filteredOphold as { title, image, subtitle, dato, afrejse, pris, undervisning, varig }}
      <Ophold
        {image}
        {title}
        {subtitle}
        {dato}
        {afrejse}
        {pris}
        {undervisning}
        {varig}
      />
    {/each}
  {:else}
    {#each opholdData as { title, image, subtitle, dato, afrejse, pris, undervisning, varig }}
      <Ophold
        {image}
        {title}
        {subtitle}
        {dato}
        {afrejse}
        {pris}
        {undervisning}
        {varig}
      />
    {/each}
  {/if}
</main> -->
<style>
  * {
    box-sizing: border-box;
  }

  /* General Structure */
  article#alleophold {
    width: 100%;
    height: auto;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: flex-start;
    justify-content: center;
  }

  section {
    padding-top: var(--padding-sections);
    padding-bottom: var(--padding-sections);
  }
  #no-pad {
    padding-top: 0;
    padding-bottom: 0;
  }
  .hero-image {
    filter: brightness(60%);
  }

  .hero-text p {
    color: white;
  }
</style>
