<script>
  import { Parallax, ParallaxLayer } from "svelte-parallax";
  import OpholdCardsSection from "../components/opholdCardsSection.svelte";

  let parallax;
  let disabled = false;
</script>

<svelte:head><title>Forside</title></svelte:head>

<section>
  <Parallax sections={3} bind:this={parallax} {disabled}>
    <ParallaxLayer
      offset={1.5}
      rate={-2.5}
      style="display: flex; justify-content: flex-end;"
      class="maxwidthwrapper"
    >
      <img
        class="h-40 w-full object-cover md:h-3/5 md:w-3/5"
        src="../src/_images/1.jpg"
        alt="Unge glade mennesker der er med på et højskoleophold"
      />
    </ParallaxLayer>

    <ParallaxLayer
      offset={1}
      rate={2.5}
      style="display: flex; justify-content: flex-start;"
    >
      <article class="maxwidthwrapper">
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

    <ParallaxLayer rate="1">
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
			justify-content: center; 
			align-items: center;
		"
    >
      <section class="maxwidthwrappper">
        <p class="preh2">MANGE SPÆNDENDE DESTINATIONER</p>
        <h2>SE VORES EVENTYRLIGE HØJSKOLEOPHOLD</h2>
        <OpholdCardsSection />
      </section>
    </ParallaxLayer>

    <ParallaxLayer
      offset="2"
      rate="2"
      style="
			display: flex; 
			justify-content: center; 
			align-items: center;
		"
    >
      <section id="statistik_sektion" class="maxwidthwrappper">
        <h2 class="center">ELSKET AF 2.500+ ELEVER</h2>
        <div>
          <h3>4,8</h3>
          <p>PÅ TRUSTPILOT</p>
        </div>
        <div>
          <h3>16</h3>
          <p>ADVENTUREFYLDTE DESTINATIONER</p>
        </div>
        <div>
          <h3>106.785</h3>
          <p>KVADRATMETER FREDET REGNSKOV TIL BEVARELSE AF VERDENS SKOVE</p>
        </div>
      </section>
    </ParallaxLayer>
  </Parallax>
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
    position: fixed;
    bottom: 3rem;
    color: #f1f1f1;
    width: 100%;
    padding: 20px;
    text-align: center;
  }

  #statistik_sektion h3 {
    color: #122554;
  }
</style>
