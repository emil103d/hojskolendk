<script>
  import Ophold_afrejse from "../components/ophold_afrejse.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section class="maxwidthwrapper" id="no-pad">
    <h2 class="">AFREJSEDATOER</h2>
    <p>
      Når vi ikke arbejder, nyder vi stranden, drikker lækre drinks på
      Rumrunners eller snorkler efter havskildpadder. Derudover har vi haft en
      masse fede ting som fx Jeepsafari i den dybe regnskov, snorkling ved Buck
      Island og turtlewatch på programmet.
    </p>

    <br />
    <hr class="py-5" />

    <section class="grid gap-8" id="no-inner-pad">
      <h4>2022</h4>
      <div class="grid gap-8">
        <Ophold_afrejse
          dato="06. Jul 2022"
          pris="29.000 DKK"
          varig="3 måneder"
        />
        <Ophold_afrejse
          dato="06. Sep 2022"
          pris="29.700 DKK"
          varig="3 måneder"
        />
        <Ophold_afrejse
          dato="06. Dec 2022"
          pris="31.400 DKK"
          varig="3 måneder"
        />
      </div>

      <h4>2023</h4>
      <div class="grid gap-8">
        <Ophold_afrejse
          dato="02. Mar 2023"
          pris="31.900 DKK"
          varig="3 måneder"
        />
        <Ophold_afrejse dato="04. Apr 2023" pris="32.700" varig="3 måneder" />
        <Ophold_afrejse dato="05. Maj 2023" pris="33.00" varig="3 måneder" />
      </div>
    </section>
  </section>
</main>

<style>
  main {
    background-image: url(src/_icons/gurfers.png);
    background-position: cover;
    background-size: 500%;
    background-repeat: repeat-y;
    background-position-y: 10%;
  }
  section {
    padding-top: var(--spacing-80);
    padding-bottom: var(--spacing-80);
  }

  #no-pad {
    padding-top: 0;
  }

  #no-inner-pad {
    padding-left: 0;
    padding-right: 0;
  }
</style>
