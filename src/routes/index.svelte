<script>
  import { Parallax, ParallaxLayer } from "svelte-parallax";

  let parallax;
  let disabled = false;
  let fancy = "fancy".split("");
</script>

<svelte:head><title>Forside</title></svelte:head>
<body>
  <Parallax sections={3} bind:this={parallax} {disabled}>
    {#each fancy as char, index (index)}
      <ParallaxLayer
        rate={(index + 1) / (fancy.length - 1)}
        offset={1}
        style="
			  margin-left: {38 + index * 5}%; 
				display: flex; 
				justify-content: flex-start; 
				align-items: center;
		  "
      >
        <p class="fancy">
          {char}
        </p>
      </ParallaxLayer>
    {/each}

    <ParallaxLayer
      offset={1}
      rate={-2.5}
      style="display: flex; justify-content: flex-end;"
    >
      <img
        class="h-42 w-full object-cover md:h-2/5 md:w-2/5"
        src="../src/_images/1.jpg"
        alt="Unge glade mennesker der er med på et højskoleophold"
      />
    </ParallaxLayer>

    <ParallaxLayer
      offset={1}
      rate={2.5}
      style="display: flex; justify-content: flex-start;"
    >
      <article class="max-w-sm">
        <h4>HVEM ER VI</h4>
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

      <button
        class="bottom-btn"
        on:click={() =>
          parallax.scrollTo(3, { selector: ".top-btn", duration: 4000 })}
      >
        Click me!
      </button>
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
      <section>
        <h4>HVEM ER VI</h4>
        <h2>HÖJSKOLENDK LEVERER ONLY GOOD VIBES OG ET FÆLLESKAB FOR LIVET</h2>
      </section>
    </ParallaxLayer>
    <button
      class="top-btn"
      on:click={() =>
        parallax.scrollTo(1, { selector: ".bottom-btn", duration: 1000 })}
    >
      Scroll to top
    </button>
  </Parallax>
</body>

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
</style>
