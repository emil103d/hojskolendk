<script>
  import PrimaryButton from "./primarybutton.svelte";
</script>

<section class="buynow flex flex-wrap flex-row gap-40">
  <div><p class="">SRI LANKA, MALDIVERNE & THAILAND</p></div>
  <div class="flex flex-row gap-10">
    <div class="linediv" />
    <div class="w-10 h-10">
      <img src="src/_icons/calender.png" alt="flyafgang ikon" />
    </div>
    <div class="grid-col-1">
      <p><strong>Varighed</strong></p>
      <p>3 måneder</p>
    </div>
    <div class="flex flex-row gap-10">
      <div class="linediv" />
      <div class="w-10 h-10">
        <img src="src/_icons/calender.png" alt="flyafgang ikon" />
      </div>
      <div class="grid-col-1">
        <p><strong>Undervisning</strong></p>
        <p>
          Selvudvikling <br />
          Kommunikation
        </p>
      </div>
    </div>
    <div><PrimaryButton>TILMELD OPHOLD</PrimaryButton></div>
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
  }

  @media screen and (max-width: 500px) {
    .buynow {
      background-color: aquamarine;
    }
  }
</style>
