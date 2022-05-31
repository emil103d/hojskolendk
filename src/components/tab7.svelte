<script>
  import Carouselle_fri from "../components/carouselle_friuge.svelte";
  import Card from "../components/card.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section class="w-full" id="">
    <h2>FRIUGER</h2>
    <p>
      Når vi ikke arbejder, nyder vi stranden, drikker lækre drinks på
      Rumrunners eller snorkler efter havskildpadder. Derudover har vi haft en
      masse fede ting som fx Jeepsafari i den dybe regnskov, snorkling ved Buck
      Island og turtlewatch på programmet.
    </p>
  </section>

  

  <!-- SECTION 2 -->
  <section class="">
    <div class="overflow-hidden">
      <p class="preh2 text-center">MALDIVERNE</p>
      <h3 class="display text-center">FRIUGE 1</h3>
      <p class="text-center">Eventyr, frihed og massere af oplevelser</p>
      <Carouselle_fri />
    </div>
  </section>

</main>

<style>
  .display {
    font-family: var(--h2_text);
    font-size: var(--font_h2);
    color: var(--sort);
    line-height: var(--line-m);
    padding: var(--spacing-10);
  }
</style>
