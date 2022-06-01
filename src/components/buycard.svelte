<script>
  import MyButton from "./button.svelte";
</script>

<section class="fixed bottom-0 left-0 bg-white drop-shadow-2xl z-50 w-[100vw] h-20">

  <div class="flex justify-evenly maxwidthwrapper_card my-5">
    
    <div class="w-full hidden md:block my-auto">
      <h4><strong>REJS TIL SRI LANKA, MALDIVERNE & THAILAND</strong></h4>
    </div>

    <div class="flex justify-center md:justify-end gap-6">
        <MyButton type="primary">BOOK REJSE</MyButton>
        <MyButton type="secondary">INFOMØDE</MyButton>
    </div>

  </div>

</section>

<style>

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
