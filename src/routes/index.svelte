<script>
  import { Parallax, ParallaxLayer } from "svelte-parallax";
  import OpholdCardsSection from "../components/opholdCardsSection.svelte";
  import CardTrustpilot from "../components/card_trustpilot.svelte";

  let parallax;
  let disabled = false;
</script>

<svelte:head><title>Forside</title></svelte:head>

<section>
  <Parallax sections={4} bind:this={parallax} {disabled}>
    <ParallaxLayer
      offset={1.5}
      rate={-2.5}
      style="display: flex; justify-content: flex-end;"
      class=""
    >
      <img
        class="h-40 w-40 md:mr-32 mr-10 object-cover md:h-3/5 md:w-3/5"
        src="../src/_images/1.jpg"
        alt="Unge glade mennesker der er med på et højskoleophold"
      />
    </ParallaxLayer>

    <ParallaxLayer
      offset={1}
      rate={2.5}
      style="display: flex; justify-content: flex-start;"
    >
      <article class="max-w-md ml-10 md:ml-32">
        <p class="preh2">HVEM ER VI</p>
        <h2>HÖJSKOLENDK LEVERER ONLY GOOD VIBES OG ET FÆLLESKAB FOR LIVET</h2>
        <p>
          Det bobler af spansk temperament, følelser og salsa rytmer i Puerto
          Rico. Hovedbyen San Juan rummer både de gamle farvede bygninger og det
          nyere arkitektur med skyskrabere. Øen er amerikansk, men er ikke noget
          man ligger mærke til, da det spanske dominerer. Her er masser af lækre
          strande, oplevelser, shopping, nightlife og adventure, og prisniveauet
          er overkommeligt.Det bobler af spansk temperament, følelser og salsa
          rytmer i Puerto Rico. Hovedbyen San Juan rummer både de gamle farvede
          bygninger og det nyere arkitektur med skyskrabere.
        </p>
        <a href="/#">Læs mere</a>
      </article>
    </ParallaxLayer>

    <ParallaxLayer offset="1" rate="-0.1">
      <img
        src="../src/_icons/buda.png"
        alt=""
        style="width: 40%; margin-left: 55%;"
      />
    </ParallaxLayer>

    <ParallaxLayer rate="2">
      <div>
        <video autoplay muted loop id="myVideo">
          <source src="../src/_video/herofrontpage.mp4" type="video/mp4" />
        </video>

        <div class="content">
          <p>Rejs med HÖJSKOLENDK</p>
          <h1>OG BLIV EN DEL AF FÆLLESKABET OG KOM PÅ DIT LIVS EVENTYR</h1>
        </div>
      </div>
    </ParallaxLayer>

    <ParallaxLayer
      offset="2"
      rate="2"
      style="
		  background-color: #faf0dc; 
			display: flex; 
			justify-content: flex-start;
			align-items: center;
		"
    >
      <section class="">
        <div class="maxwidthwrappper">
          <p class="preh2">MANGE SPÆNDENDE DESTINATIONER</p>
          <h2>SE VORES EVENTYRLIGE HØJSKOLEOPHOLD</h2>
          <OpholdCardsSection />
          <button>SE ALLE OPHOLD</button>
        </div>
      </section>
    </ParallaxLayer>

    <ParallaxLayer
      offset="2.8"
      rate="0.5"
      style="
			display: flex; 
			justify-content: flex-start;
			align-items: center;
		"
    >
      <section
        id="statistik_sektion"
        class="maxwidthwrappper text-center w-full"
      >
        <h2 class="mb-5">ELSKET AF 2.500+ ELEVER</h2>
        <div class="flex gap-10 mx-auto justify-center">
          <div class="max-w-xs">
            <h3>4,8</h3>
            <p>PÅ TRUSTPILOT</p>
            <img class="w-40" src="../src/_icons/5star.png" alt="" />
          </div>
          <div class="max-w-xs">
            <h3>16</h3>
            <p>ADVENTUREFYLDTE DESTINATIONER</p>
          </div>
          <div class="max-w-xs">
            <h3>106.785</h3>
            <p>KVADRATMETER FREDET REGNSKOV TIL BEVARELSE AF VERDENS SKOVE</p>
          </div>
        </div>
      </section>
    </ParallaxLayer>
  </Parallax>
</section>

<section class="maxwidthwrappper">
  <p class="preh2">VI ELSKER VORES ELEVER OG VORES ELEVER ELSKER OS</p>
  <h2>VORES ELEVER PÅ TRUSTPILOT</h2>
  <img src="../src/_logo/trustpilot_logo.png" alt="" />
  <div class="flex gap-5 mt-10 m-5 mx-auto justify-center">
    <CardTrustpilot
      title="Venskaber for livet"
      text="vil du venskaber og gode oplevelser i god kombi med en meget tryg rejseoplevelse, så synes jeg du skal investere i dig selv og købe en højskolerejse med HÖJSKOLENDK"
      image="../src/_images/2.jpg"
      name=" Camilla Jensen"
    />
    <CardTrustpilot
      image="../src/_images/2.jpg"
      title="Fantastisk rejse"
      name=" Camilla Jensen"
      text="
Mit ophold med HÖJSKOLENDK var noget af det bedste, jeg har gjort for mig selv i mit liv. Jeg oplevede stor professionalisme og ansvarlighed fra organisationens side, og mine rejseledere var enormt kompetente, jordnære og skabte stor tryghed i gruppen."
    />

    <CardTrustpilot
      image="../src/_images/2.jpg"
      title="Fantastisk rejse"
      name=" Camilla Jensen"
      text="

Jeg oplevede et fællesskab, jeg ikke sidenhen har prøvet, og jeg fik venskaber med mig for livet. Og så var det en stor udviklingsrejse både gennem undervisningen men lige så meget ved friheden til at rejse på egen hånd og stå på egne ben."
    />
  </div>
</section>

<style>
  /* Style the video: 100% width and height to cover the entire window */
  #myVideo {
    position: fixed;
    right: 0;
    bottom: 0;
    min-width: 100%;
    min-height: 100%;
  }

  /* Add some content at the bottom of the video/page */
  .content {
    position: relative;
    z-index: 5;
    bottom: -12rem;
    color: #f1f1f1;
    width: 100%;
    padding: 20px;
    text-align: center;
  }

  #statistik_sektion {
    background-image: url(../src/_icons/airplane_earth.png);
    background-repeat: no-repeat;
    background-position: center;
    background-size: 80%;
    padding-bottom: 10rem;
  }

  #statistik_sektion h3 {
    color: #122554;
    font-family: var(--h1_text);
    font-size: 8rem;
  }
</style>
