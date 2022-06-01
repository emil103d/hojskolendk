<script>
  import MyButton from "../components/button.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section
    itemscope
    itemtype="https://schema.org/Product"
    class="maxwidthwrapper grid gap-5"
    id="no-pad"
  >
    <div>
      <h2 itemprop="keywords">SURF, SOL & BEACH VIBES</h2>
      <p itemprop="description">
        Når vi ikke arbejder, nyder vi stranden, drikker lækre drinks på
        Rumrunners eller snorkler efter havskildpadder. Derudover har vi haft en
        masse fede ting som fx Jeepsafari i den dybe regnskov, snorkling ved
        Buck Island og turtlewatch på programmet.
      </p>
      <br />
      <hr />
    </div>
  </section>

  <!-- SECTION 2 -->
  <!-- <section class="maxwidthwrapper">
    <div
      class="container grid grid-cols-2 grid-rows-2 lg:grid-rows-1 lg:grid-cols-4 gap-2 text-center"
    >
      <div class="col-start-1 row-start-1 infobokse">
        <img
          class="h-8 w-auto m-auto"
          src="src/_icons/destination.png"
          alt=""
        />
        <h4>Destinationer</h4>
        <p class="table">Sri Lanka, Maldiverne & Thailand</p>
      </div>
      <div class="col-start-2 row-start-1 infobokse">
        <img class="h-8 w-auto m-auto" src="src/_icons/calender.png" alt="" />
        <h4>Varighed</h4>
        <p>3 måneder</p>
      </div>
      <div
        class="col-start-1 row-start-2 lg:col-start-3 lg:row-start-1 infobokse"
      >
        <img class="h-8 w-auto m-auto" src="src/_icons/faelleskab.png" alt="" />
        <h4>Undervisning</h4>
        <p>Selvudvikling & Kommunikation</p>
      </div>
      <div
        class="col-start-2 row-start-2 lg:row-start-1 lg:col-start-4 infobokse "
      >
        <img class="h-8 w-auto m-auto" src="src/_icons/price.png" alt="" />
        <h4>Pris</h4>
        <p>59.700 DKK</p>
      </div>
    </div>
  </section> -->

  <!-- SECTION 3 -->

  <section class="maxwidthwrapper">
    <div
    class=" grid grid-cols-2 grid-rows-2 lg:grid-rows-1 lg:grid-cols-4 gap-2 text-center"
  >
    <div class="col-start-1 row-start-1 infobokse">
      <img
        class="h-8 w-auto m-auto"
        src="src/_icons/destination.png"
        alt="map ikon"
      />
      <p class="infoboks_tekst">Destinationer</p>
      <p itemprop="name" class="table">Sri Lanka, Maldiverne & Thailand</p>
    </div>
    <div class="col-start-2 row-start-1 infobokse">
      <img
        class="h-8 w-auto m-auto"
        src="src/_icons/calender.png"
        alt="kalender ikon"
      />
      <p class="infoboks_tekst">Varighed</p>
      <p>3 måneder</p>
    </div>
    <div
      class="col-start-1 row-start-2 lg:col-start-3 lg:row-start-1 infobokse"
    >
      <img
        class="h-8 w-auto m-auto"
        src="src/_icons/faelleskab.png"
        alt="fælleskab ikon"
      />
      <p class="infoboks_tekst">Undervisning</p>
      <p>Selvudvikling & Kommunikation</p>
    </div>
    <div
      itemprop="offers"
      itemscope
      itemtype="https://schema.org/Offer"
      class="col-start-2 row-start-2 lg:row-start-1 lg:col-start-4 infobokse "
    >
      <img
        class="h-8 w-auto m-auto"
        src="src/_icons/price.png"
        alt="pris ikon"
      />
      <p class="infoboks_tekst">Pris</p>
      <p itemprop="price">59.700 DKK</p>
    </div>
  </div>

  </section>

  

  <section class="maxwidthwrapper" itemscope="" itemtype="https://schema.org/Trip">
    <div class="grid align-middle">
      <div class="">
        <p itemprop="name">HVAD DER VENTER FORUDE</p>
        <h2 itemprop="description">OVERBLIK</h2>
      </div>

      <div class="grid custom_grid baggrund-klode">
        <div />
        <div
          class="rejseplan overflow-scroll overflow-x-hidden max-h-[30vh] max-w-[500px] relative p-4 grid gap-7"
        >
          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 1</b> <br />
                  Introdage i Dubai
                </p>
              </div>
            </div>
          </div>

          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 2</b> <br />
                  Projektstyring & teambuilding
                </p>
              </div>
            </div>
          </div>

          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 3</b> <br />
                  Friuge med aktiviteter
                </p>
              </div>
            </div>
          </div>

          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 4</b> <br />Projektstyring & Teambuilding
                  
                </p>
              </div>
            </div>
          </div>

          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 5</b> <br />Friuge på egen hånd
                  
                </p>
              </div>
            </div>
          </div>

          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 6</b> <br />Selvudvikling og kommunikation
                  
                </p>
              </div>
            </div>
          </div>

          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 7</b> <br />Selvudvikling og kommunikation
                  
                </p>
              </div>
            </div>
          </div>


          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 8</b> <br />Selvudvikling og kommunikation
                  
                </p>
              </div>
            </div>
          </div>

          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 9</b> <br />Friuge på egen hånd
                  
                </p>
              </div>
            </div>
          </div>

          <div itemprop="subTrip">
            <div class="flex gap-2 items-center">
              <img class="h-8" src="src/_icons/destination.png" alt="" />
              <div class="ml-2">
                <p class="leading-tight">
                  <b>Uge 10</b> <br />Outrotur
                  
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- SECTION 4 -->
  <section class="maxwidthwrapper">
    <p class="preh2">ER DU NYSGERRIG</p>
    <h2>FØLG OPHOLDET DIREKTE @ MLSBG_HDK</h2>
    <div class="grid grid-rows-3 sm:grid-cols-3 lg:grid-cols-4">
      <img
        class="sm:row-start-1 sm:col-start-1 lg:col-start-1 object-cover w-full aspect-square"
        src="src/_images/webp/dykke.webp"
        alt=""
      />
      <img
        class="sm:row-start-1 sm:col-start-2 lg:col-start-2 object-cover w-full aspect-square"
        src="src/_images/webp/riverraft.webp"
        alt=""
      />
      <img
        class="sm:row-start-1 sm:col-start-3 lg:col-start-3 object-cover w-full aspect-square"
        src="src/_images/webp/social.webp"
        alt=""
      />
      <img
        class="sm:row-start-1 sm:col-start-1 hidden sm:grid lg:col-start-4 object-cover w-full aspect-square"
        src="src/_images/webp/solnedgang.webp"
        alt=""
      />
      <img
        class="sm:row-start-2 sm:col-start-2 hidden sm:grid lg:col-start-1 object-cover w-full aspect-square"
        src="src/_images/webp/surf.webp"
        alt=""
      />
      <img
        class="sm:row-start-2 sm:col-start-3 hidden sm:grid lg:col-start-2 object-cover w-full aspect-square"
        src="src/_images/webp/social4.webp"
        alt=""
      />
      <img
        class="sm:row-start-2 sm:col-start-1 hidden sm:grid lg:col-start-3 object-cover w-full aspect-square"
        src="src/_images/webp/rapelvandfald.webp"
        alt=""
      />
      <img
        class="sm:row-start-2 sm:col-start-2 hidden sm:grid lg:col-start-4 object-cover w-full aspect-square"
        src="src/_images/webp/social5.webp"
        alt=""
      />
      <img
        class="sm:row-start-3 sm:col-start-3 hidden sm:grid lg:col-start-1 object-cover w-full aspect-square"
        src="src/_images/webp/riverrafting4.webp"
        alt=""
      />
      <img
        class="sm:row-start-3 sm:col-start-1 hidden sm:grid lg:col-start-2 object-cover w-full aspect-square"
        src="src/_images/webp/social9.webp"
        alt=""
      />
      <img
        class="sm:row-start-3 sm:col-start-2 hidden sm:grid lg:col-start-3 object-cover w-full aspect-square"
        src="src/_images/webp/social13.webp"
        alt=""
      />
      <img
        class="sm:row-start-3 sm:col-start-3 hidden sm:grid lg:col-start-4 object-cover w-full aspect-square"
        src="src/_images/webp/social12.webp"
        alt=""
      />
    </div>

    <div />
  </section>



<!-- 
  <section class="flex justify-end px-4">
    <MyButton type="linkbutton">  HVAD ER INKLUDERET<svg class="m-auto" width="18" height="16" viewBox="0 0 18 16" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M17.7071 8.70711C18.0976 8.31658 18.0976 7.68342 17.7071 7.29289L11.3431 0.928932C10.9526 0.538408 10.3195 0.538408 9.92893 0.928932C9.53841 1.31946 9.53841 1.95262 9.92893 2.34315L15.5858 8L9.92893 13.6569C9.53841 14.0474 9.53841 14.6805 9.92893 15.0711C10.3195 15.4616 10.9526 15.4616 11.3431 15.0711L17.7071 8.70711ZM17 7L-4.76837e-07 7V9L17 9V7Z" fill="#929292"/>
      </svg>
       </MyButton> 
  </section> -->
</main>

<style>
  main {
    background-image: url(src/_icons/gurfers.png);
    background-position: cover;
    background-size: 280%;
    background-repeat: no-repeat;
    background-position-y: 60%;
  }
  .infobokse {
    background-color: var(--sandbeach);
    display: grid;
    place-content: center;
    gap: 0.3rem;
    padding: 2rem;
  }

  .baggrund-klode {
    background-image: url(src/_images/verdenskort_m_destinationer.png);
    background-position: 50%;
    background-position-y: 40%;
    padding-top: 2rem;
    padding-bottom: 2rem;
    background-size: contain;
    background-repeat: no-repeat;
    background-size: 100%;
  }

  .custom_grid {
    grid-template-columns: auto 400px;
  }

  .table {
    font-size: var(--font_p_table);
  }

  section {
    padding-top: var(--padding-sections);
    padding-bottom: var(--padding-sections);
  }

  .rejseplan {
    background-color: var(--sandbeach);
  }

  #no-pad {
    padding-top: 0;
  }

  .infoboks_tekst {
    font-size: var(--font_h4);
    color: var(--txtcolor);
  }
</style>
