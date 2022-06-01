<script>
  import MyButton from "../components/button.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section class="maxwidthwrapper" id="no-pad">
    <h2>UNDERVISNINGEN</h2>
    <p>
      Når vi ikke arbejder, nyder vi stranden, drikker lækre drinks på
      Rumrunners eller snorkler efter havskildpadder. Derudover har vi haft en
      masse fede ting som fx Jeepsafari i den dybe regnskov, snorkling ved Buck
      Island og turtlewatch på programmet.
    </p>
    <br />
    <hr />
  </section>

  <!-- SECTION 2 -->
  <section class="lg:grid md:grid-cols-2 maxwidthwrapper">
    <div class="lg:col-start-1 lg:pr-8 grid place-content-center">
      <div class="">
        <p>FAG 1:</p>
        <h4>SELVUDVIKLING & KOMMUNIKATION</h4>
        <p>
          Lörem ipsum får kende. Tredons bida dir rödgrönrosa. Sona dotivis. Eda
          bokstav bejåligt. Heminade abel oaktat prest. Nekes kolertad
          genuskänslig.Lörem ipsum får kende. Tredons bida dir rödgrönrosa. Sona
          dotivis. Eda bokstav bejåligt. Heminade abel oaktat prest. bejåligt.
          Heminade abel oaktat prest.
        </p>
        <button>Læs mere</button>
      </div>
    </div>
    <div class="lg:col-start-2">
      <img
        class="object-cover w-full aspect-square"
        src="src/_images/sogk.jpg"
        alt=""
      />
    </div>
  </section>

  <!-- SECTION 3 -->
  <section class="lg:grid md:grid-cols-2 md:grid-rows-1 maxwidthwrapper">
    <div
      class="lg:col-start-2 lg:row-start-1 lg:pl-8 grid place-content-center"
    >
      <div>
        <p>FAG 2:</p>
        <h4>PROJEKTSTYRING & TEAMBUILDING</h4>
        <p>
          Lörem ipsum får kende. Tredons bida dir rödgrönrosa. Sona dotivis. Eda
          bokstav bejåligt. Heminade abel oaktat prest. Nekes kolertad
          genuskänslig.Lörem ipsum får kende. Tredons bida dir rödgrönrosa. Sona
          dotivis. Eda bokstav bejåligt. Heminade abel oaktat prest. bejåligt.
          Heminade abel oaktat prest.
        </p>
        <button>Læs mere</button>
      </div>
    </div>
    <div class="lg:col-start-1 lg:row-start-1">
      <img
        class="object-cover w-full aspect-square"
        src="src/_images/pogt.jpg"
        alt=""
      />
    </div>
  </section>

  <!-- SECTION 4 -->
  <section class="lg:grid md:grid-cols-2 maxwidthwrapper">
    <div class="lg:col-start-1 lg:pr-8 grid place-content-center">
      <div>
        <p>FAG 3:</p>
        <h4>SPORT & ADVENTURE</h4>
        <p>
          Lörem ipsum får kende. Tredons bida dir rödgrönrosa. Sona dotivis. Eda
          bokstav bejåligt. Heminade abel oaktat prest. Nekes kolertad
          genuskänslig.Lörem ipsum får kende. Tredons bida dir rödgrönrosa. Sona
          dotivis. Eda bokstav bejåligt. Heminade abel oaktat prest. bejåligt.
          Heminade abel..
        </p>
        <button>Læs mere</button>
      </div>
    </div>
    <div class="lg:col-start-2">
      <img
        class="object-cover w-full aspect-square "
        src="src/_images/soga.jpg"
        alt=""
      />
    </div>
  </section>

  <section class="flex justify-end px-4">
    <MyButton type="linkbutton"> AFREJSEDATOER -> </MyButton> 
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
    padding-top: var(--padding-sections);
    padding-bottom: var(--padding-sections);
  }

  #no-pad {
    padding-top: 0;
  }
</style>
