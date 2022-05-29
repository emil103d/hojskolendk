<script>
  import PrimaryButton from "./primarybutton.svelte";
</script>

<section class="flex flex-row">
  <div><p>SRI LANKA, MALDIVERNE & THAILAND</p></div>
  <div>
    <div class="grid-col-1">
      <p><strong>Varighed</strong></p>
      <p>3 måneder</p>
    </div>
    <div><img src="src/_icons/calender.png" alt="flyafgang ikon" /></div>
    <div class="linediv" />
  </div>
  <div><PrimaryButton>TILMELD OPHOLD</PrimaryButton></div>
</section>

<style>
  .linediv {
    height: 10px;
    width: 1px;
    background-color: var(--txtcolor);
  }
</style>
