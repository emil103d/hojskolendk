<script>
  import MyButton from "../components/button.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section class="maxwidthwrapper" id="no-pad">
    <h2>MØD DIN REJSELEDER</h2>
    <div class="baggrundsfarve">
      <div class="xl:grid custom_grid">
        <div class="lg:col-start-1">
          <img
            class="w-full h-full object-cover"
            src="anton.webp"
            alt="Billede af din rejseleder"
          />
        </div>
        <div
          class="lg:col-start-2 lg:col-span-2 p-6 lg:p-10 m-auto max-w-[50ch]"
        >
          <h3 class="pb-4">Anton Skou Larsen</h3>
          <p>
            Jeg har, siden jeg var ganske lille, haft stor lyst og trang til at
            udforske verden. Jeg har altid været interesseret i naturen; gåture
            i skove og være ved vandet med forestillinger om at der lå verdener
            uden for min forstand. Der er altid mere eventyr i horisonten, når
            man ser på verden gennem mine briller. Jeg drømmer om at komme alle
            de steder hen i verden, jeg endnu ikke har været (og der er
            heldigvis mange), og tror på, at respekt og kærlighed for andre
            mennesker, opstår i mødet og kendskabet med deres kultur og
            verdensforståelse. Jeg har rejst siden jeg var 15 år gammel, på både
            små-ture til Sverige i et par uger ad gangen og som 17-årig begav
            jeg mig alene ud i Europa, hvor jeg tomlede den til Sydspanien, og
            bagefter fløj til Island og drog hele vejen rundt på den smukke, rå
            og vilde vulkanø. Det var første gang jeg for alvor kom i kontakt
            med det, der fylder mig mest med glæde som menneske; at rejse og
            møde mennesker på tværs af landegrænser.

            <br />
            <br />
            Højskolesmil, <br /> Anton
          </p>
        </div>
      </div>
    </div>
  </section>
</main>

<style>
  main {
    background-image: url("../../boys.png");
    background-position: cover;
    background-size: 200%;
    background-repeat: repeat-y;
    background-position-y: 10%;
  }
  .baggrundsfarve {
    background-color: var(--sandstone);
  }

  .custom_grid {
    grid-template-columns: 1fr auto;
  }

  section {
    padding-top: var(--padding-sections);
    padding-bottom: var(--padding-sections);
  }

  #no-pad {
    padding-top: 0;
  }
</style>
