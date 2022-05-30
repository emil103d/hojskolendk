<script>
  export let varig;
  export let pris;
  export let dato;
  import PrimaryButton from "./primarybutton.svelte";
  import SecondaryButton from "./secondarybutton.svelte";
</script>

<section class="ophold text-center p-6 md:flex">
  <div class="md:flex hidden">
    <div>
      <img
        class="w-12 h-12 mr-5 justify-center items-center"
        src="../src/_icons/calender.png"
        alt=""
      />
      <div>
        <p class="">Afrejse:</p>
        <p class="tabeltxt">{dato}</p>
      </div>
    </div>
    <div class="h-full w-0.5 bg-black" />
  </div>
  <div class="md:block">
    <h3 class="pt-5">Sri Lanka, Maldiverne & Thailand</h3>
    <div class="grid grid-cols-2">
      <div class="flex items-center">
        <div class="flex">
          <div class="flex mt-5">
            <img class="w-8 h-8 mr-5" src="../src/_icons/calender.png" alt="" />
            <div>
              <div>
                <p class="">Varighed:</p>
                <p class="tabeltxt text-left">{varig}</p>
              </div>
            </div>
          </div>
          <div class="flex mt-5">
            <img class="w-8 h-8 mr-5" src="../src/_icons/price.png" alt="" />
            <div>
              <div class="justify-start">
                <p class="">Pris:</p>
                <p class="tabeltxt text-left">{pris}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="h-24 bg-black w-0.5 ml-3 mr-6 md:hidden" />
    </div>
  </div>
  <div class=" ">
    <div class="block">
      <PrimaryButton>TILMELD</PrimaryButton>
    </div>
    <div class="">
      <SecondaryButton>RESERVER</SecondaryButton>
    </div>
  </div>
</section>

<section class="ophold">
  <div class="">
    <img class="w-8 h-8 mr-5" src="../src/_icons/calender.png" alt="" />
    <div>
      <p class="">Afrejse:</p>
      <p class="tabeltxt">{dato}</p>
    </div>
    <div class="h-full w-5 bg-black" />
  </div>
  <div>
    <h1>Sri Lanka, Maldiverne & Thailand</h1>
    <div>
      <div class="flex mt-5">
        <img class="w-8 h-8 mr-5" src="../src/_icons/calender.png" alt="" />
        <div>
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
        <div>
          <button>TILMELD</button>
          <button>RESERVER</button>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .ophold {
    margin: 5px;
    background-color: var(--sandbeach);
    margin-bottom: 2rem;
  }
</style>
