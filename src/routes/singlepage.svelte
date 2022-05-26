<script>
  import TabA from "../components/tabA.svelte";
  import TabB from "../components/tabB.svelte";
  import TabC from "../components/tabC.svelte";

  let activetab = "TabA";
</script>

<main>
  <button on:click={() => (activetab = "TabA")}>Tab A</button>
  <button on:click={() => (activetab = "TabB")}>Tab B</button>
  <button on:click={() => (activetab = "TabC")}>Tab C</button>

  {#if activetab === "TabA"}
    <TabA />
  {/if}
  {#if activetab === "TabB"}
    <TabB />
  {/if}
  {#if activetab === "TabC"}
    <TabC />
  {/if}
</main>

<style>
</style>
