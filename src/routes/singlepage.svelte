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
  import Header from "../components/header.svelte";

  let activetab = Tab1;
</script>

<Header imgtitle="src/_images/1.jpg" />
<div class="m-9 preh2">
  <a href="indec">FORSIDE /</a>
  <a href="alleophold" class=" preh2">ALLE OPHOLD</a>
  <a href="alleophold" class="underline preh2">SKRI LANKA & BAli</a>
</div>

<main class="max_width_single relative">
  <section class="md:custom_grid hidden md:grid md:gap-10 lg:gap-20">
    <sidebar id="navbar" class="block cols-start-1 top-0 sticky mt-10 mb-10">
      <div class="sticky top-28">
        <h2 class="text:sm m:1 mb:6">Alt du skal vide om opholdet</h2>
        <button class="" on:click={() => (activetab = Tab1)}
          >OPHOLDSOVERSIGT</button
        >
        <button on:click={() => (activetab = Tab2)}>HVAD ER INKLUDERET</button>
        <button on:click={() => (activetab = Tab3)}>PROGRAM</button>
        <button on:click={() => (activetab = Tab4)}>UNDERVISNINGEN</button>
        <button on:click={() => (activetab = Tab5)}>AFREJSEDATOER</button>
        <button on:click={() => (activetab = Tab6)}>GODT AT VIDE</button>
        <button on:click={() => (activetab = Tab7)}>FRIUGER</button>
        <button on:click={() => (activetab = Tab8)}>ADVENTURE</button>
        <button on:click={() => (activetab = Tab9)}>REJSEBREVE</button>
        <button on:click={() => (activetab = Tab10)}>DIN REJSELEDER</button>
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

  .max_width_single {
    max-width: 1400px;
  }

  #navbar {
    top: 0;
  }
</style>
