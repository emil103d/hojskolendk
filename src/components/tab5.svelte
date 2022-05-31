<script>
  import Ophold_afrejse from "../components/ophold_afrejse.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section class="maxwidthwrapper" id="no-pad">
    <h2 class="">Afrejsedatoer</h2>
    <p>
      Når vi ikke arbejder, nyder vi stranden, drikker lækre drinks på
      Rumrunners eller snorkler efter havskildpadder. Derudover har vi haft en
      masse fede ting som fx Jeepsafari i den dybe regnskov, snorkling ved Buck
      Island og turtlewatch på programmet.
    </p>

    <section class="grid gap-8" id="no-inner-pad">
      <h4>2022</h4>
      <div class="grid gap-8">
        <Ophold_afrejse
          dato="Bali, Lombok & Gili Islands"
          pris="1500kr."
          varig="1500kr."
        />
        <Ophold_afrejse
          dato="Bali, Lombok & Gili Islands"
          pris="1500kr."
          varig="1500kr."
        />
        <Ophold_afrejse
          dato="Bali, Lombok & Gili Islands"
          pris="1500kr."
          varig="1500kr."
        />
    </div>

    <h4>2023</h4>
    <div class="grid gap-8">
      
      <Ophold_afrejse
        dato="Bali, Lombok & Gili Islands"
        pris="1500kr."
        varig="1500kr."
      />
      <Ophold_afrejse
        dato="Bali, Lombok & Gili Islands"
        pris="1500kr."
        varig="1500kr."
      />
      <Ophold_afrejse
        dato="Bali, Lombok & Gili Islands"
        pris="1500kr."
        varig="1500kr."
      />
  </div>
    </section>

  </section>
</main>

<style>
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
