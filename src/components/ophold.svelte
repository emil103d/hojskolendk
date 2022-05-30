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
  class="ophold max-w-xs md:max-w-7xl h-full block md:flex items-center mb-5"
  transition:scale={{ duration: 1000, easing: expoInOut }}
>
  <img src={image} alt={title} class="w-full object-cover md:w-40 mr-10" />
  <div>
    <div class="m-5">
      <h3>{title}</h3>
      <p>{subtitle}</p>
    </div>
    <div class="md:flex mt-10 m-5">
      <div class="flex mt-3">
        <img class="w-8 h-8 mr-6" src="../src/_icons/flyafgang.png" alt="" />
        <div class="">
          <p class="">Afrejse:</p>
          <p class="tabeltxt">{dato}</p>
        </div>
        <div class="h-10 hidden md:block bg-black w-0.5 ml-3 mr-6" />
      </div>
      <div class="flex mt-5">
        <img class="w-8 h-8 mr-5" src="../src/_icons/calender.png" alt="" />
        <div>
          <p class="">Varighed:</p>
          <p class="tabeltxt">{varig}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6 hidden md:block" />
      </div>
      <div class="flex mt-5">
        <img class="w-8 h-8 mr-5" src="../src/_icons/price.png" alt="" />
        <div>
          <p class="">Pris:</p>
          <p class="tabeltxt">{pris}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6 hidden md:block" />
      </div>
      <div class="flex mt-5 mb-5">
        <img class="w-8 h-8 mr-5" src="../src/_icons/faelleskab.png" alt="" />
        <div>
          <p class="">Undervisning:</p>
          <p class="tabeltxt">{undervisning}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6 hidden md:block" />
      </div>
    </div>
  </div>
  <div>
    <button class="right hidden md:block"
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

  @media screen and (max-width: 400px) {
    section {
      max-width: 100px;
    }
  }
</style>
