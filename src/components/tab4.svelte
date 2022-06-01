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
        <h3>SELVUDVIKLING & KOMMUNIKATION</h3>
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
        <h3>PROJEKTSTYRING & TEAMBUILDING</h3>
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
        <h3>SPORT & ADVENTURE</h3>
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
    <MyButton type="linkbutton"> AFREJSEDATOER <svg class="m-auto" width="18" height="16" viewBox="0 0 18 16" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M17.7071 8.70711C18.0976 8.31658 18.0976 7.68342 17.7071 7.29289L11.3431 0.928932C10.9526 0.538408 10.3195 0.538408 9.92893 0.928932C9.53841 1.31946 9.53841 1.95262 9.92893 2.34315L15.5858 8L9.92893 13.6569C9.53841 14.0474 9.53841 14.6805 9.92893 15.0711C10.3195 15.4616 10.9526 15.4616 11.3431 15.0711L17.7071 8.70711ZM17 7L-4.76837e-07 7V9L17 9V7Z" fill="#929292"/>
      </svg></MyButton> 
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
