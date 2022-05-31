<script>
  import MyButton from "./button.svelte";
</script>

<section class="fixed bottom-0 left-0 bg-red-600 z-50 w-[100vw] pt-5 block my-auto">
  <div class="flex justify-between maxwidthwrapper ">
    <div class="block my-auto">
      <p><strong>REJS TIL SRI LANKA, MALDIVERNE & THAILAND</strong></p>
    </div>
  
    <div class="">
      <MyButton type="primary">TILMELD OPHOLD</MyButton>
      <MyButton type="secondary">TILMELD OPHOLD</MyButton>
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
