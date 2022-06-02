<script>
  import { scale } from "svelte/transition";
  import { expoInOut } from "svelte/easing";
  export let image;
  export let title;
  export let subtitle;
  export let dato;
  export let afrejse;
  export let pris;
  export let undervisning;
  export let varig;
  import MyButton from "../components/button.svelte";
</script>

<section
  class="ophold h-auto w-full block md:flex max-w-[1400px] items-center mb-5 pb-6"
  transition:scale={{ duration: 1000, easing: expoInOut }}
>
  <div class="h-full w-auto object-cover min-w-[200px]">
    <img src={image} alt={title} class="h-full w-auto object-cover" />
  </div>
  <div>
    <div class="m-5">
      <h3>{title}</h3>
      <p>{subtitle}</p>
    </div>
    <div class="grid grid-cols-2 grid-rows-2 md:flex mt-10 m-5 gap-6">
      <div class="flex col-start-1 md: place-items-center">
        <img
          class="w-8 h-8 mr-6"
          src="../src/_icons/flyafgang.png"
          alt="flyafgangs ikon"
        />
        <div class="">
          <p class="">Næste afrejse:</p>
          <p class="tabeltxt">{dato}</p>
        </div>
        <div class="h-10 hidden md:block bg-black w-0.5 ml-3 mr-6" />
      </div>

      <div class="flex col-start-2 place-items-center ">
        <img
          class="w-8 h-8 mr-5"
          src="../src/_icons/calender.png"
          alt="ikon af kalender"
        />
        <div>
          <p class="">Varighed:</p>
          <p class="tabeltxt">{varig}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6 hidden md:block" />
      </div>

      <div class="flex col-start-1 row-start-2 place-items-center">
        <img
          class="w-8 h-8 mr-5"
          src="../src/_icons/price.png"
          alt="pris ikon"
        />
        <div>
          <p class="">Pris:</p>
          <p class="tabeltxt">{pris}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6 hidden md:block" />
      </div>

      <div class="flex col-start-2 row-start-2 place-items-center ">
        <img
          class="w-8 h-8 mr-5"
          src="../src/_icons/faelleskab.png"
          alt="fælleskab ikon"
        />
        <div>
          <p class="">Undervisning:</p>
          <p class="tabeltxt">{undervisning}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6 hidden md:block" />
      </div>
    </div>
    <div class="grid justify-center md:justify-start ml-3 pt-4">
      <MyButton type="primary">Læs mere</MyButton>
    </div>
  </div>
</section>

<style>
  .ophold {
    margin: 5px;
    background-color: var(--sandstone);
    margin-bottom: 2rem;
  }

  .right svg {
    height: 25px;
    width: 25px;
  }

  .right {
    background-color: white;
    border-radius: 50px;
    height: 60px;
    width: 60px;
    z-index: 10;
  }

  @media screen and (max-width: 400px) {
    section {
      max-width: 100px;
    }
  }
</style>
