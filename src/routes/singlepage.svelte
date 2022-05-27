<script>
  import Tab1 from "../card_trustpilot.svelte/tab1.svelte";
  import Tab2 from "../card_trustpilot.svelte/tab2.svelte";
  import Tab3 from "../card_trustpilot.svelte/tab3.svelte";
  import Tab4 from "../card_trustpilot.svelte/tab4.svelte";
  import Tab5 from "../card_trustpilot.svelte/tab5.svelte";
  import Tab6 from "../card_trustpilot.svelte/tab6.svelte";
  import Tab7 from "../card_trustpilot.svelte/tab7.svelte";
  import Tab8 from "../card_trustpilot.svelte/tab8.svelte";
  import Tab9 from "../card_trustpilot.svelte/tab9.svelte";
  import Tab10 from "../card_trustpilot.svelte/tab10.svelte";

  let activetab = Tab1;
</script>

<main>
  <section class="grid-cols-5 hidden md:grid lg:gap-20">
    <sidebar id="navbar" class="block cols-start-1">
      <h2 class="text:sm m:1 mb:6">Alt du skal vide om opholdet</h2>
      <button class="" on:click={() => (activetab = Tab1)}
        >OPHOLDSOVERSIGT</button
      >
      <button on:click={() => (activetab = Tab2)}>HVAD ER INKLUDERET</button>
      <button on:click={() => (activetab = Tab3)}>PROGRAM</button>
      <button on:click={() => (activetab = Tab4)}>UNDERVISNINGEN</button>
      <button on:click={() => (activetab = Tab5)}>AFREJSEDATOER</button>
      <button on:click={() => (activetab = Tab6)}>DOGT AT VIDE</button>
      <button on:click={() => (activetab = Tab7)}>FRIUGER</button>

      <button on:click={() => (activetab = Tab8)}>ADVENTURE</button>
      <button on:click={() => (activetab = Tab9)}>REJSEBREVE</button>
      <button on:click={() => (activetab = Tab10)}>DIN REJSELEDER</button>
    </sidebar>
    <svelte:component this={activetab} />
    <!-- {#if activetab === "TabA"}
        <TabA />
      {/if}
      {#if activetab === "TabB"}
        <TabB />
      {/if}
      {#if activetab === "TabC"}
        <TabC />
      {/if} -->
  </section>

  <section class="sticky overflow-hidden md:hidden block">
    <sidebar class="block">
      <h2 class="text:sm m:1 mb:6 ml-auto text-center">
        Alt du skal vide om opholdet
      </h2>
      <div class="flex overflow-x-scroll pb-10 flex-nowrap overflow-hidden">
        <div class="flex flex-nowrap  ">
          <button class="" on:click={() => (activetab = Tab1)}
            >OPHOLDSOVERSIGT</button
          >
          <button on:click={() => (activetab = Tab2)}>HVAD ER INKLUDERET</button
          >
          <button on:click={() => (activetab = Tab3)}>PROGRAM</button>
          <button on:click={() => (activetab = Tab4)}>UNDERVISNINGEN</button>
          <button on:click={() => (activetab = Tab5)}>AFREJSEDATOER</button>
          <button on:click={() => (activetab = Tab6)}>DOGT AT VIDE</button>
          <button on:click={() => (activetab = Tab7)}>FRIUGER</button>

          <button on:click={() => (activetab = Tab8)}>ADVENTURE</button>
          <button on:click={() => (activetab = Tab9)}>REJSEBREVE</button>
          <button on:click={() => (activetab = Tab10)}>DIN REJSELEDER</button>
        </div>
      </div>
    </sidebar>
    <svelte:component this={activetab} />
    <!-- {#if activetab === "TabA"}
        <TabA />
      {/if}
      {#if activetab === "TabB"}
        <TabB />
      {/if}
      {#if activetab === "TabC"}
        <TabC />
      {/if} -->
  </section>
</main>

<style>
  button {
    border-bottom: 2px solid #545454;
    min-width: 12rem;
    text-align: left;
    margin: 1rem;
    display: inline-block;
    overflow: hidden;
  }

  #navbar button {
    display: block;
  }

  button:focus,
  button:hover {
    border-bottom: 2px solid #545454;
    font-weight: 800;
  }
</style>
