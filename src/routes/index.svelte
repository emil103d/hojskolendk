<script>
  import CardTrustpilot from "../components/card_trustpilot.svelte";
  import Card from "../components/card.svelte";
  import MyButton from "../components/button.svelte";
  import Cookie from "../components/cookie.svelte";
  import Chat from "../components/chat.svelte";
  import Saos from "saos";
  let cookie;

  function handleObserver(x) {
    console.info(x.detail.observing);
  }
</script>

<header class="h-full w-full relative overflow-hidden" id="video">
  <video class="z-0 hero-image" loop muted autoplay src="herofrontpage.mp4" />
  <div class="hero-text m-auto">
    <p class="text-white">HØJSKOLEOPHOLD I UDLANDET</p>
    <h1 class="">FÆLLESKAB & REJSEEVENTYR</h1>
  </div>

  <div class="wave absolute bottom-[6px]">
    <svg
      width="3311"
      height="69"
      viewBox="0 0 3311 69"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M1117.7 32.6112C407.753 27.7762 99.6691 49.7522 0 66.7752V69L170.798 67.9949H640.254H3311V32.6112V0C3214.82 13.0946 2921.85 49.8962 2519.46 56.1817C2016.46 64.0384 2005.13 38.6548 1117.7 32.6112Z"
        fill="white"
      />
    </svg>
  </div>
</header>

<!-- section #1 start -->
<section class="maxwidthwrapper md:pt-0 md:grid md:justify-center md:gap-8">
  <article class="cols-start-1 grid items-center place-items-center">
    <div class="grid md:grid-cols-2 md:gap-10 lg:gap-20">
      <div class="grid md:block md:m-auto">
        <div class="rows-start-1">
          <Saos
            animation={"from-left 0.9s cubic-bezier(0.35, 0.5, 0.65, 0.95) both"}
          >
            <p class="preh2">PÅ HØJSKOLE I UDLANDET</p>
          </Saos>

          <Saos
            animation={"from-left 1s cubic-bezier(0.35, 0.5, 0.65, 0.95) both"}
          >
            <h2>
              REJSEEVENTYR, SOMMER VIBES & <br /> ET FÆLLESSKAB I VERDENSKLASSE
            </h2>
          </Saos>
        </div>

        <Saos
          animation={"from-left 1.4s cubic-bezier(0.35, 0.5, 0.65, 0.95) both"}
        >
          <div class="row-start-3 md:row-auto">
            <p class="pb-6">
              HÖJSKOLENDK er noget for dig, hvis du vil på højskole i udlandet
              og er vild med højskolefællesskab, vil med på et fantastisk
              rejseeventyr, glæder dig til at lære om fremmede kulturer, vil
              rejse med rygsæk, drømmer om en fed grupperejse med andre skønne
              unge, vil opleve et stærkt sammenhold og ønsker inspirerende og
              meningsfuld undervisning. Du er sikker på en tryg rejseoplevelse
              da vi er medlem af Rejsegarantifonden.
            </p>
          </div>
        </Saos>
        <Saos
          animation={"slide-in-fwd-tr 1.3s cubic-bezier(0.250, 0.460, 0.450, 0.940) both"}
        >
          <div class="row-start-4 md:row-auto">
            <MyButton type="primary">JOIN OS TIL INFOMØDE</MyButton>
          </div>
        </Saos>

        <div class="rows-start-2 pb-6 md:row-auto md:hidden">
          <img
            class=""
            src="sektion1.webp"
            alt="Unge glade mennesker der er med på et højskoleophold"
          />
        </div>
      </div>

      <div class="hidden md:grid md:m-auto">
        <Saos
          animation={"slide-in-fwd-tr 0.6s cubic-bezier(0.250, 0.460, 0.450, 0.940) both"}
        >
          <img
            class=""
            src="../src/_images/webp/sektion1.webp"
            alt="Unge glade mennesker der er med på et højskoleophold"
          />
        </Saos>
      </div>
    </div>
  </article>
</section>

<!-- section #1 slut -->

<section id="section_2">
  <div class="maxwidthwrapper">
    <p class="preh2">MANGE SPÆNDENDE DESTINATIONER</p>
    <h2 class="">SE VORES EVENTYRLIGE HØJSKOLEOPHOLD</h2>
    <div
      class="flex justify-between gap-5 overflow-hidden hover:overflow-x-scroll"
    >
      <Card
        image="../src/_images/webp/ophold1.webp"
        title="Maldiverne, Sri Lanka, Bali & Gili"
      />
      <Card
        image="../src/_images/webp/ophold2.webp"
        title="Bali, Lombok & Gili Islands"
      />
      <Card
        image="../src/_images/webp/ophold3.webp"
        title="Caribien, Hawaii & Mexico"
      />
      <Card
        image="../src/_images/webp/ophold4.webp"
        title="Costa Rica, Mexico & Guatemala"
      />
    </div>
    <div class="md:justify-center md:grid pt-6">
      <MyButton type="primary">UDFORSK ALLE VORES OPHOLD</MyButton>
    </div>
  </div>
</section>

<!-- section #2 Start -->

<section class="maxwidthwrapper mx-auto pb-0">
  <div class="">
    <p class="preh2">ELSKET AF 2500+ ELEVER</p>
    <h2>SE VORES ANMELDELSER</h2>
    <img
      class="md:bg-contain"
      src="../src/_logo/trustpilot_logo.png"
      alt="truspilot logo"
    />
    <div class="md:flex grid gap-16 md:gap-5 mt-10 mx-auto justify-around">
      <CardTrustpilot
        title="Venskaber for livet"
        text="vil du venskaber og gode oplevelser i god kombi med en meget tryg rejseoplevelse, så synes jeg du skal investere i dig selv og købe en højskolerejse med HÖJSKOLENDK. du vil aldrig du vil aldrig fortryde eller glemme det. afsted !"
        image="../src/_images/webp/social3.webp"
        name=" Jackie Salomonsen"
      />

      <CardTrustpilot
        image="../src/_images/webp/social4.webp"
        title="Fantastisk rejse"
        name=" Camilla Jensen"
        text="
Mit ophold med HÖJSKOLENDK var noget af det bedste, jeg har gjort for mig selv i mit liv. Jeg oplevede stor professionalisme og ansvarlighed fra organisationens side, og mine rejseledere var enormt kompetente, jordnære og skabte stor tryghed i gruppen."
      />

      <div class="hidden lg:grid">
        <CardTrustpilot
          image="../src/_images/webp/social6.webp"
          title="Uforglemmeligt"
          name=" Søren Reves"
          text="

    Jeg oplevede et fællesskab, jeg ikke sidenhen har prøvet, og jeg fik venskaber med mig for livet. Og så var det en stor udviklingsrejse både gennem undervisningen men lige så meget ved friheden til at rejse på egen hånd og stå på egne ben."
        />
      </div>
    </div>
  </div>
</section>

<!-- Statistik sektion start -->
<section
  id=""
  class="statistik_sektion maxwidthwrapper text-center w-full md:p-64 min-h-[35vh] grid items-center justify-center"
>
  <Saos
    animation={"puff-in-center 0.7s cubic-bezier(0.470, 0.000, 0.745, 0.715) both"}
    animation_out={"slide-out-elliptic-top-bck 0.7s ease-in both"}
    top={250}
    bottom={250}
    on:update={handleObserver}
  >
    <div class="">
      <h2 class="mb-5 hidden">ELSKET AF 2.500+ ELEVER</h2>

      <div
        class="grid gap-6 md:flex md:gap-40 md:mx-auto md:justify-center airplane"
      >
        <div class="md:max-w-xs">
          <p class=" text-black ">2.500+</p>
          <h5>TIDLIGERE ELEVER ELSKER OS</h5>
        </div>

        <div class="md:max-w-xs">
          <p class=" text-black">4,8</p>
          <h5>PÅ TRUSTPILOT</h5>
          <img
            class="w-80"
            src="../src/_icons/5star.png"
            alt="4,8 stjerne på trustpilot"
          />
        </div>

        <div class="md:max-w-xs">
          <p class=" text-black">106.785</p>
          <h5 class="max-w-xs m-auto">M2 FREDET REGNSKOV</h5>
        </div>
      </div>
    </div>
  </Saos>
</section>

<section class="maxwidthwrapper">
  <p class="preh2">WE'RE SOCIAL</p>
  <h2>FØLG VORES REJSEEVENTYR @ HÖJSKOLENDK</h2>
  <div class="grid grid-rows-3 sm:grid-cols-3 lg:grid-cols-4">
    <img
      class="sm:row-start-1 sm:col-start-1 lg:col-start-1 object-cover w-full aspect-square"
      src="src/_images/webp/dykke.webp"
      alt="instagram - dykker hopper i vandet"
    />
    <img
      class="sm:row-start-1 sm:col-start-2 lg:col-start-2 object-cover w-full aspect-square"
      src="src/_images/webp/riverraft.webp"
      alt="instagram - kajak tur"
    />
    <img
      class="sm:row-start-1 sm:col-start-3 lg:col-start-3 object-cover w-full aspect-square"
      src="src/_images/webp/social.webp"
      alt="instagram - Surfing"
    />
    <img
      class="sm:row-start-1 sm:col-start-1 hidden sm:grid lg:col-start-4 object-cover w-full aspect-square"
      src="src/_images/webp/solnedgang.webp"
      alt="instagram - Hygge i golden hour"
    />
    <img
      class="sm:row-start-2 sm:col-start-2 hidden sm:grid lg:col-start-1 object-cover w-full aspect-square"
      src="src/_images/webp/surf.webp"
      alt="instagram - Surfing"
    />
    <img
      class="sm:row-start-2 sm:col-start-3 hidden sm:grid lg:col-start-2 object-cover w-full aspect-square"
      src="src/_images/webp/social4.webp"
      alt="instagram - Piger der sidder på en gren i vandkanten"
    />
    <img
      class="sm:row-start-2 sm:col-start-1 hidden sm:grid lg:col-start-3 object-cover w-full aspect-square"
      src="src/_images/webp/rapelvandfald.webp"
      alt="instagram - Rapelle ned af vandfald"
    />
    <img
      class="sm:row-start-2 sm:col-start-2 hidden sm:grid lg:col-start-4 object-cover w-full aspect-square"
      src="src/_images/webp/social5.webp"
      alt="instagram - Glade piger på tur"
    />
    <img
      class="sm:row-start-3 sm:col-start-3 hidden sm:grid lg:col-start-1 object-cover w-full aspect-square"
      src="src/_images/webp/riverrafting4.webp"
      alt="instagram - river rafting tur"
    />
    <img
      class="sm:row-start-3 sm:col-start-1 hidden sm:grid lg:col-start-2 object-cover w-full aspect-square"
      src="src/_images/webp/social9.webp"
      alt="instagram - højt humør og drinks"
    />
    <img
      class="sm:row-start-3 sm:col-start-2 hidden sm:grid lg:col-start-3 object-cover w-full aspect-square"
      src="src/_images/webp/social13.webp"
      alt="instagram - dykker med nissehuer"
    />
    <img
      class="sm:row-start-3 sm:col-start-3 hidden sm:grid lg:col-start-4 object-cover w-full aspect-square"
      src="src/_images/webp/social12.webp"
      alt="instagram - Alle elever har pakket tasker"
    />
  </div>
</section>

<!-- Statistik section  slut -->

<!-- sectCookie og Chation  -->

<Cookie bind:this={cookie}>
  <button
    on:click={() => {
      cookie.closeModal();
    }}>Close dialog</button
  >
</Cookie>

<Chat />

<style>
  section {
    overflow: hidden;
    padding-top: var(--spacing-80);
    padding-bottom: var(--spacing-80);
  }

  #section_2 {
    background-color: var(--sandbeach);
  }

  .wave svg {
    margin-bottom: -10px;
    overflow: hidden;
    width: 100vw;
    height: auto;
    margin-bottom: -8px;
  }

  .wave {
    height: auto;
    width: 100vw;
    object-fit: contain;
  }

  #section_2 svg {
    margin: auto;
  }

  .statistik_sektion {
    background-image: url(../src/_icons/airplane_earth.png);
    background-size: contain;
    background-position: 50%;
    background-repeat: no-repeat;
    height: 65vh;
  }

  #statistik_sektion h3 {
    color: #122554;
    font-family: var(--h1_text);
    font-size: var(--font_talsek);
  }
  #statistik_sektion img {
    width: 200px;
    margin: 0 auto;
  }
  .airplane p {
    font-family: "Prociono", serif;
    font-size: var(--font_figur);
  }

  /* article {
    max-width: 700px;
  } */

  /* ANIMATIONER */

  /* Sektion 1 artikel animation */
  @keyframes -global-from-left {
    0% {
      transform: rotateX(50deg) translateX(-200vw) skewX(-50deg);
      opacity: 1;
    }
    100% {
      transform: rotateX(0deg) translateX(0) skewX(0deg);
      opacity: 1;
    }
  }

  /* Billede animation */
  @keyframes -global-slide-in-fwd-tr {
    0% {
      transform: translateY(1000px);
      opacity: 0;
    }
    100% {
      transform: translateY(0);
      opacity: 1;
    }
  }

  /* Tekst animation */

  @keyframes -global-tracking-in-contract {
    0% {
      letter-spacing: 1em;
      opacity: 0;
    }
    40% {
      opacity: 0.6;
    }
    100% {
      letter-spacing: normal;
      opacity: 1;
    }
  }

  /* Rotate */
  @keyframes -global-rotate-in-center {
    0% {
      transform: rotate(-360deg);
      opacity: 0;
    }
    100% {
      transform: rotate(0);
      opacity: 1;
    }
  }

  .rotate_animation:hover {
    animation: rotate-in-center 0.6s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;
  }

  @keyframes -global-puff-in-center {
    0% {
      transform: scale(2);
      filter: blur(4px);
      opacity: 0;
    }
    100% {
      transform: scale(1);
      filter: blur(0px);
      opacity: 1;
    }
  }

  @keyframes tilt-in-top-1 {
    0% {
      transform: rotateY(30deg) translateY(-300px) skewY(-30deg);
      opacity: 0;
    }
    100% {
      transform: rotateY(0deg) translateY(0) skewY(0deg);
      opacity: 1;
    }
  }
</style>
