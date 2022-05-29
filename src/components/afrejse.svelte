<script>
  export let afrejse;
  export let selectedAf;
  $: console.log(afrejse);
</script>

<!-- svelte-ignore a11y-no-onchange -->

<ul class="menu-cont mt-10">
  <select class="menu" name="menu" id="afrejseselektor" bind:value={selectedAf}>
    <option disabled selected value="">Afrejse</option>
    <option value="all">All afrejser</option>
    {#each afrejse as af}
      <option value={af}>{af}</option>
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
    border-bottom: 1px solid gray;
  }

  .menu {
    width: 40%;
  }
</style>
