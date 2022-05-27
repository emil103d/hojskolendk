<script>
  import Tab1 from "../components/tab1.svelte";
  import Tab2 from "../components/tab2.svelte";
  import Tab3 from "../components/tab3.svelte";
  import Tab4 from "../components/tab4.svelte";
  import Tab5 from "../components/tab5.svelte";
  import Tab6 from "../components/tab6.svelte";
  import Tab7 from "../components/tab7.svelte";
  import Tab8 from "../components/tab8.svelte";
  import Tab9 from "../components/tab9.svelte";
  import Tab10 from "../components/tab10.svelte";

  let activetab = Tab1;
</script>

<main>
  <section class=" grid-cols-2 sm:hidden md:grid">
    <sidebar id="navbar" class="block">
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

  <section class="sticky overflow-hidden md:hidden sm:display">
    <sidebar class="block">
      <h2 class="text:sm m:1 mb:6 ml-auto text-center">
        Alt du skal vide om opholdet
      </h2>
      <div class="flex overflow-x-scroll pb-10 flex-nowrap overflow-hidden">
        <div class="flex flex-nowrap lg:ml-40 md:ml-20 ml-10 ">
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
