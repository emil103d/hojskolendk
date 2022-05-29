<script>
  import { onMount } from "svelte";
  import Header from "../components/header.svelte";
  import { opholdData } from "../stores/opholdData.js";
  import Menu from "../components/menu.svelte";
  import Afrejseselekt from "../components/afrejse.svelte";
  import Ophold from "../components/ophold.svelte";

  let varighed = []; // menu built from opholdData
  let afrejse = []; // afrejse built from opholdData
  let selectedvar = ""; //  menu selection
  let selectedAf = ""; //  menu selection

  const getVarigheder = () => {
    for (let opholdObj of opholdData) {
      if (!varighed.includes(opholdObj.varig)) {
        varighed = [...varighed, opholdObj.varig];
      }
    }
    varighed = varighed.sort();
  };
  onMount(() => getVarigheder());

  const getAfrejser = () => {
    for (let opholdObj of opholdData) {
      if (!afrejse.includes(opholdObj.af)) {
        afrejse = [...afrejse, opholdObj.af];
      }
    }
    afrejse = afrejse.sort();
  };
  onMount(() => getAfrejser());

  // Query results
  let filteredOphold = [];

  // For Select Menu
  $: if (selectedvar) getOpholdByVar();
  $: console.log(filteredOphold, selectedvar);

  $: if (selectedAf) getOpholdByVar();
  $: console.log(filteredOphold, selectedAf);

  const getOpholdByVar = () => {
    if (selectedvar === "all") {
      return (filteredOphold = []);
    }
    return (filteredOphold = opholdData.filter(
      (ophold) => ophold.varig === selectedvar || ophold.af === selectedvar
    ));
  };
</script>

<Header imgtitle="src/_images/1.jpg" />
<div class="m-9 preh2">
  <a href="indec">FORSIDE /</a>
  <a href="alleophold" class="underline preh2">ALLE OPHOLD</a>
</div>

<section class="maxwidthwrapper text-center justify-center">
  <h2>Hvor drømmer du om at rejse hen?</h2>
  <p>
    Drømmer du om et friår fra studierne, en pause fra udannelsesræsset eller
    bare har lyst til et opleve verdenen? Så dyk ned og læs mere om vores
    spændende højskoleophold og tag med os ud og udfroske verdenen!
  </p>
  <div class="flex mt-10 mb-10 justify-center ml-auto mr-auto">
    <Menu {varighed} bind:selectedvar />
    <Afrejseselekt {afrejse} bind:selectedAf />
  </div>
</section>

<main id="alleophold">
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
</main>

<style>
  * {
    box-sizing: border-box;
  }

  /* General Structure */
  main#alleophold {
    width: 90%;
    justify-content: center;
  }
</style>
