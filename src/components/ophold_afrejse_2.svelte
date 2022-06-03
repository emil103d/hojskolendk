<script>
  export let varig;
  export let pris;
  export let dato;
  import MyButton from "./button.svelte";
</script>

<section
  class="background_color_boks p-4 md:m-0 lg:flex lg:justify-around lg:p-4 lg:items-center md:p-0"
>
  <div class="hidden lg:grid lg:text-center lg:justify-items-center">
    <img
      class="w-12 h-12 md:block"
      src=".calender.png"
      alt="ikon af kalender"
    />
    <h3>Afrejse</h3>
    <p class="tabeltxt">{dato}</p>
  </div>

  <div class="grid justify-center py-4 lg:p-0">
    <h3>Sri Lanka, Maldiverne & Thailand</h3>

    <div class="flex gap-8 lg:gap-12 pt-4 justify-center lg:justify-start">
      <div class="flex items-center gap-2">
        <img class="w-8 h-8" src="calender.png" alt="ikon af kalender" />
        <div>
          <p class="font-bold">Varighed</p>
          <p class="tabeltxt">{varig}</p>
        </div>
      </div>

      <div class="hidden">
        <img class="w-8 h-8 " src="calender.png" alt="ikon af kalender" />
        <p class="font-bold">Afrejse</p>
        <p class="tabeltxt">{dato}</p>
      </div>

      <div class="h-full w-0.5 bg-black" />

      <div class="flex items-center gap-2">
        <img class="w-8 h-8" src="calender.png" alt="ikon af kalender" />
        <div>
          <p class="font-bold">Pris</p>
          <p class="tabeltxt">{pris}</p>
        </div>
      </div>
    </div>
  </div>
  <div class="flex lg:grid lg:grid-rows-2 justify-center py-4 gap-8 lg:gap-4">
    <MyButton type="primary">TILMELD</MyButton>
    <MyButton type="secondary">RESERVER</MyButton>
  </div>
</section>

<style>
  .background_color_boks {
    background-color: var(--sandstone);
  }
</style>
