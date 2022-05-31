<script>
  import MyButton from "./button.svelte";
</script>

<section class="pr-8 pl-8 fixed bottom-0 left-0 bg-red z-50 w-[100vw]">
  <div class="flex justify-between maxwidthwrapper">
    <div>
      <p><strong>REJS TIL SRI LANKA, MALDIVERNE & THAILAND</strong></p>
    </div>
  
    <div class="pl-4">
      <MyButton type="primary">TILMELD OPHOLD</MyButton>
      <MyButton type="secondary">TILMELD INFOMØDE</MyButton>
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
