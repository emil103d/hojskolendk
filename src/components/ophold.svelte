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
  export let varighed;
</script>

<section
  class="ophold block md:flex"
  transition:scale={{ duration: 1000, easing: expoInOut }}
>
  <img src={image} alt={title} class="w-60 mr-10" />
  <div>
    <div>
      <h3>{title}</h3>
      <p>{subtitle}</p>
    </div>
    <div class="md:flex mt-10">
      <div class="flex">
        <img class="w-10 h-10 mr-5" src="../src/_icons/flyafgang.png" alt="" />
        <div>
          <p class="">Afrejse:</p>
          <p>{dato}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6" />
      </div>
      <div class="flex">
        <img class="w-10 h-10 mr-5" src="../src/_icons/flyafgang.png" alt="" />
        <div>
          <p class="">Varighed:</p>
          <p>{varighed}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6" />
      </div>
      <div class="flex">
        <img class="w-10 h-10 mr-5" src="../src/_icons/flyafgang.png" alt="" />
        <div>
          <p class="">Pris:</p>
          <p>{pris}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6" />
      </div>
      <div class="flex">
        <img class="w-10 h-10 mr-5" src="../src/_icons/flyafgang.png" alt="" />
        <div>
          <p class="">Undervisning:</p>
          <p>{undervisning}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6" />
      </div>
    </div>
  </div>
  <div>
    <button>Next</button>
  </div>
</section>

<style>
  .ophold {
    margin: 5px;
    background-color: var(--sandbeach);
  }
</style>
