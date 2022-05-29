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
</script>

<section
  class="ophold block md:flex items-center"
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
        <img class="w-10 h-10 mr-5" src="../src/_icons/calender.png" alt="" />
        <div>
          <p class="">Varighed:</p>
          <p>{varig}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6" />
      </div>
      <div class="flex">
        <img class="w-10 h-10 mr-5" src="../src/_icons/price.png" alt="" />
        <div>
          <p class="">Pris:</p>
          <p>{pris}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6" />
      </div>
      <div class="flex">
        <img class="w-10 h-10 mr-5" src="../src/_icons/faelleskab.png" alt="" />
        <div>
          <p class="">Undervisning:</p>
          <p>{afrejse}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6" />
      </div>
    </div>
  </div>
  <div>
    <button class="right"
      ><svg
        width="43"
        height="66"
        viewBox="0 0 43 66"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M2.95605 2.92773L37.8401 34.2031L2.95605 63.0727"
          stroke="black"
          stroke-width="6"
        />
      </svg>
    </button>
  </div>
</section>

<style>
  .ophold {
    margin: 5px;
    background-color: var(--sandbeach);
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
</style>
