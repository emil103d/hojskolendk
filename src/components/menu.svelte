<script>
  export let varighed;
  export let selectedvar;
  $: console.log(varighed);
</script>

<ul class="menu-cont mt-10">
  <select class="menu" name="menu" id="menu" bind:value={selectedvar}>
    <option disabled selected value="">Varighed</option>
    <!-- Alle valgmuligheder option -->
    <option value="all">Alle varigheder</option>
    <!-- Tilføjer alle varighed options -->
    {#each varighed as varig}
      <option value={varig}>{varig}</option>
    {/each}
  </select>
</ul>

<style>
  .menu-cont {
    width: 150px;
    display: flex;
    margin: 0 10px 0 0;
  }
  select {
    margin: 0;
    font-size: 1.18rem;
    border-bottom: 1px solid gray;
  }
  .menu {
    width: 150px;
    background-color: var(--sandstone);
    padding-top: 0.5rem;
  }
</style>
