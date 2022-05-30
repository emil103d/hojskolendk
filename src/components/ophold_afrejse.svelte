<script>
  export let varig;
  export let pris;
  export let dato;
  import PrimaryButton from "./primarybutton.svelte";
  import SecondaryButton from "./secondarybutton.svelte";
</script>


<section class="background_color_boks p-4 m-4 md:m-0 lg:flex lg:justify-around lg:p-4 lg:items-center md:p-0">
  
  
    <div class="hidden lg:grid lg:text-center lg:justify-items-center">
      <img class="w-12 h-12 md:block" src="../src/_icons/calender.png" alt="" />
      <h3>Afrejse</h3>
      <p class="tabeltxt">{dato}</p>
    </div>

    

    <div class="grid justify-center py-4 lg:p-0">
      <h3>Sri Lanka, Maldiverne & Thailand</h3>
      
      <div class="flex gap-6 pt-4">
        
        <div class="flex items-center gap-2">
          <img class="w-8 h-8" src="../src/_icons/calender.png" alt="" />
          <div>
            <p class="font-bold">Varighed </p>
            <p class="tabeltxt">{dato}</p>
          </div>
        </div>

        <div class="hidden">
          <img class="w-8 h-8 " src="../src/_icons/calender.png" alt="" />
          <p class="font-bold">Afrejse </p>
          <p class="tabeltxt">{varig}</p>
        </div>

        <div class="h-full w-0.5 bg-black" />

        <div class="flex items-center gap-2">
          <img class="w-8 h-8" src="../src/_icons/calender.png" alt="" />
          <div>
            <p class="font-bold">Pris </p>
            <p class="tabeltxt">{pris}</p>
          </div>
        </div>
      
      </div>
    </div>
    <div class="flex lg:grid lg:grid-rows-2 justify-center py-4 gap-8 lg:gap-4">
      <PrimaryButton>TILMELD</PrimaryButton>
      <SecondaryButton>RESERVER</SecondaryButton>
    </div>

</section>

<style>
  .background_color_boks {
    background-color: var(--sandstone);
  }
</style>




