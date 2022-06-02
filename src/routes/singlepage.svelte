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
  import BuyCard from "../components/buycard.svelte";

  // function current() {
  //   document.getElementById("demo").style.fontWeight = "400";
  //   document.getElementById("demo").style.fontWeight = "900";
  // }

  let current = "1";

  let activetab = Tab1;
</script>

<Header imgtitle="src/_images/webp/ferie2.webp" />
<div class="m-9 preh2">
  <a href="index">Forside /</a>
  <a href="alleophold" class=" preh2">Alle ophold /</a>
  <a href="alleophold" class="underline preh2"
    >Sri Lanka, Maldiverne & Thailand
  </a>
</div>

<main class="max_width_single relative">
  <section class="md:custom_grid hidden md:grid md:gap-10 lg:gap-20">
    <sidebar id="navbar" class="block cols-start-1 top-0 sticky">
      <div class="sticky top-28 pb-16">
        <h2 class="text:sm m:1 mb:6 w-[237px]">
          ALT DU SKAL VIDE <br /> OM OPHOLDET
        </h2>
        <button
          class={current === "1" ? "selected" : ""}
          on:click={() => (current = "1")}
          on:click={() => (activetab = Tab1)}
          >OPHOLDSOVERSIGT
        </button>
        <button
          class={current === "2" ? "selected" : ""}
          on:click={() => (current = "2")}
          on:click={() => (activetab = Tab2)}>HVAD ER INKLUDERET</button
        >
        <button
          class={current === "3" ? "selected" : ""}
          on:click={() => (current = "3")}
          on:click={() => (activetab = Tab3)}>PROGRAM</button
        >
        <button
          class={current === "4" ? "selected" : ""}
          on:click={() => (current = "4")}
          on:click={() => (activetab = Tab4)}>UNDERVISNINGEN</button
        >
        <button
          class={current === "5" ? "selected" : ""}
          on:click={() => (current = "5")}
          on:click={() => (activetab = Tab5)}>AFREJSEDATOER</button
        >
        <button
          class={current === "6" ? "selected" : ""}
          on:click={() => (current = "6")}
          on:click={() => (activetab = Tab6)}>GODT AT VIDE</button
        >
        <button
          class={current === "7" ? "selected" : ""}
          on:click={() => (current = "7")}
          on:click={() => (activetab = Tab7)}>FRIUGER</button
        >
        <button
          class={current === "8" ? "selected" : ""}
          on:click={() => (current = "8")}
          on:click={() => (activetab = Tab8)}>ADVENTURE</button
        >
        <button
          class={current === "9" ? "selected" : ""}
          on:click={() => (current = "9")}
          on:click={() => (activetab = Tab9)}>REJSEBREVE</button
        >
        <button
          class={current === "10" ? "selected" : ""}
          on:click={() => (current = "10")}
          on:click={() => (activetab = Tab10)}>DIN REJSELEDER</button
        >
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
    <sidebar class="block pb-10">
      <h2 class="text:sm m:1 mb:6 ml-auto text-center">
        Alt du skal vide om opholdet
      </h2>
      <div class="flex overflow-x-scroll flex-nowrap overflow-hidden">
        <div class="flex flex-nowrap  ">
          <button class="" on:click={() => (activetab = Tab1)}
            >OPHOLDSOVERSIGT</button
          >
          <button on:click={() => (activetab = Tab2)}>HVAD ER INKLUDERET</button
          >
          <button on:click={() => (activetab = Tab3)}>PROGRAM</button>
          <button on:click={() => (activetab = Tab4)}>UNDERVISNINGEN</button>
          <button on:click={() => (activetab = Tab5)}>AFREJSEDATOER</button>
          <button on:click={() => (activetab = Tab6)}>GODT AT VIDE</button>
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

  <BuyCard />
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

  .selected {
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
