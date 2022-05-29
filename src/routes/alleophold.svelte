<script>
  import { onMount } from "svelte";

  import { opholdData } from "../stores/opholdData.js";
  import Menu from "../components/menu.svelte";
  import Ophold from "../components/ophold.svelte";

  let languages = []; // menu built from opholdData
  let selectedLang = ""; //  menu selection

  const getLanguages = () => {
    for (let bookObj of opholdData) {
      if (!languages.includes(bookObj.language)) {
        languages = [...languages, bookObj.language];
      }
    }
    languages = languages.sort();
  };
  onMount(() => getLanguages());

  // Query results
  let filteredBooks = [];

  // For Select Menu
  $: if (selectedLang) getBooksByLang();
  $: console.log(filteredBooks, selectedLang);

  const getBooksByLang = () => {
    if (selectedLang === "all") {
      return (filteredBooks = []);
    }
    return (filteredBooks = opholdData.filter(
      (ophold) => ophold.language === selectedLang
    ));
  };
</script>

<section>
  <h2>Hvor drømmer du om at rejse hen?</h2>
  <p>
    Drømmer du om et friår fra studierne, en pause fra udannelsesræsset eller
    bare har lyst til et opleve verdenen? Så dyk ned og læs mere om vores
    spændende højskoleophold og tag med os ud og udfroske verdenen!
  </p>
</section>

<section id="query-section">
  <Menu {languages} bind:selectedLang />
</section>

<main id="alleophold">
  {#if filteredBooks.length > 0}
    {#each filteredBooks as { title, image, subtitle, dato, afrejse, pris, undervisning, varighed }}
      <Ophold
        {image}
        {title}
        {subtitle}
        {dato}
        {afrejse}
        {pris}
        {undervisning}
        {varighed}
      />
    {/each}
  {:else}
    {#each opholdData as { title, image, subtitle, dato, afrejse, pris, undervisning, varighed }}
      <Ophold
        {image}
        {title}
        {subtitle}
        {dato}
        {afrejse}
        {pris}
        {undervisning}
        {varighed}
      />
    {/each}
  {/if}
</main>

<style>
  * {
    box-sizing: border-box;
  }

  #query-section {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 2% 0;
  }

  /* General Structure */
  main#alleophold {
    width: 100%;
    margin: 10px;
    justify-content: center;
  }
</style>
