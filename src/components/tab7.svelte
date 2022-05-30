<script>
  import Carouselle_fri from "../components/carouselle_friuge.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section>
    <h2>Friuger</h2>
    <p>
      Når vi ikke arbejder, nyder vi stranden, drikker lækre drinks på
      Rumrunners eller snorkler efter havskildpadder. Derudover har vi haft en
      masse fede ting som fx Jeepsafari i den dybe regnskov, snorkling ved Buck
      Island og turtlewatch på programmet.
    </p>
  </section>

  <!-- SECTION 2 -->
  <section class="lg:grid md:grid-cols-2">
    <div class="lg:col-start-1">
      <p class="preh2">ADVENTURE I FRIUGEN</p>
      <h4>FRIUGE 1- Maldiverne</h4>
      <p>Uendelige oplevelser og muligheder</p>
      <Carouselle_fri />
    </div>
    <div class="lg:col-start-2">
      <img class="w-full h-auto" src="src/_images/program_1.png" alt="" />
    </div>
  </section>
</main>

<style>
</style>
