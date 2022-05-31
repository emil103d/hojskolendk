<script>
  import MyButton from "./button.svelte";
</script>

<section class="pr-8 pl-8 fixed bottom-0 left-0 bg-white z-50 w-[100vw]">
  <div class="flex flex-row gap-8 justify-center">
    <div><p><strong>REJS TIL SRI LANKA, MALDIVERNE & THAILAND</strong></p></div>
    <div class="hidden lg:flex lg:flex-row  lg:gap-10">
      <div class="linediv" />
      <div class="w-10 h-10">
        <img src="src/_icons/calender.png" alt="flyafgang ikon" />
      </div>
      <div class="grid-col-1 ">
        <p><strong>Varighed</strong></p>
        <p>3 måneder</p>
      </div>
      <div class="flex flex-row gap-10">
        <div class="linediv" />
        <div class="w-10 h-10">
          <img src="src/_icons/faelleskab.png" alt="flyafgang ikon" />
        </div>
        <div class="grid-col-1">
          <p><strong>Undervisning</strong></p>
          <p>
            Selvudvikling & <br />
            Kommunikation
          </p>
        </div>
      </div>
    </div>
    <div class="pl-4">
      <MyButton type="primary">TILMELD OPHOLD</MyButton>
      <MyButton type="secondary">TILMELD OPHOLD</MyButton>
    </div>
  </div>
</section>

<style>
  * {
    margin: auto;
  }
  .linediv {
    height: 60px;
    width: 1px;
    background-color: var(--txtcolor-600);
  }

  p {
    font-weight: 100;
    font-size: var(--font_knap_s);
  }
</style>
