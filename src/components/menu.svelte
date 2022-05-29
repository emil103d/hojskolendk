<script>
  export let languages;
  export let selectedLang;
  // $:console.log(languages)
</script>

<!-- svelte-ignore a11y-no-onchange -->

<ul class="menu-cont mt-10">
  <select class="menu" name="menu" id="menu" bind:value={selectedLang}>
    <option disabled selected value="">Varighed</option>
    <option value="all">Varighed</option>
    {#each varighed as varig}
      <option value={varighed}>{varighed}</option>
    {/each}
  </select>
</ul>

<style>
  .menu-cont {
    width: 40%;
    display: flex;
    margin: 0 10px 0 0;
  }

  select {
    margin: 0;
    font-size: 1.18rem;
    border: 1px solid gray;
    border-radius: 5px;
  }

  .menu {
    width: 100%;
  }
</style>
