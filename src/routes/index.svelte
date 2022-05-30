<script>
  import CardTrustpilot from "../components/card_trustpilot.svelte";
  import Card from "../components/card.svelte";
  import PrimaryButton from "../components/primarybutton.svelte"
</script>

<header class="h-full w-full"id="video">
  <video
    class="z-0 hero-image"
    loop
    muted
    autoplay
    src="../src/_video/herofrontpage.mp4"
  />
  <div class="hero-text m-auto">
    <p>Rejs med HÖJSKOLENDK</p>
    <h1 class="">OG BLIV EN DEL AF FÆLLESKABET OG KOM PÅ DIT LIVS EVENTYR</h1>
  </div>
</header>

<!-- section #1 start -->
<section
  class="maxwidthwrapper md:pt-0 md:flex md:justify-center md:gap-8"
>
  <article class="">
    <p class="preh2">VI ER</p>
    <h2>REJSEEVENTYR, SOMMER VIBES & ET FÆLLESSKAB I VERDENSKLASSE</h2>
    <p>
      HÖJSKOLENDK er noget for dig, hvis du vil på højskole i udlandet og er
      vild med højskolefællesskab, vil med på et fantastisk rejseeventyr, glæder
      dig til at lære om fremmede kulturer, vil rejse med rygsæk, drømmer om en
      fed grupperejse med andre skønne unge, vil opleve et stærkt sammenhold og
      ønsker inspirerende og meningsfuld undervisning. Du er sikker på en tryg
      rejseoplevelse da vi er medlem af Rejsegarantifonden.
    </p>
    <button>JOIN OS TIL INFOMØDE</button>
  </article>
  <div>
    <img
      class=""
      src="../src/_images/webp/sektion1.webp"
      alt="Unge glade mennesker der er med på et højskoleophold"
    />
  </div>
</section>
<!-- section #1 slut -->

<section id="section_2" >
  <div class="maxwidthwrapper">
    <p class="preh2">MANGE SPÆNDENDE DESTINATIONER</p>
    <h2 class="">SE VORES EVENTYRLIGE HØJSKOLEOPHOLD</h2>
    <div class="flex justify-center gap-5 hover:overflow-x-scroll">
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
    <PrimaryButton>UDFORSK ALLE VORES OPHOLD</PrimaryButton>

  </div>
</section>

<!-- section #2 Start -->
<section class="maxwidthwrapper mx-auto mx-4 pb-0">
  <p class="preh2">VI ELSKER VORES ELEVER OG VORES ELEVER ELSKER OS</p>
  <h2>VORES ELEVER PÅ TRUSTPILOT</h2>
  <img src="../src/_logo/trustpilot_logo.png" alt="" />
  <div class="md:flex grid gap-16 md:gap-5 mt-10 m-5 mx-auto justify-center">
    <CardTrustpilot
      title="Venskaber for livet"
      text="vil du venskaber og gode oplevelser i god kombi med en meget tryg rejseoplevelse, så synes jeg du skal investere i dig selv og købe en højskolerejse med HÖJSKOLENDK"
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
    <CardTrustpilot
      image="../src/_images/webp/social6.webp"
      title="Uforglemmeligt"
      name=" Søren Reves"
      text="

Jeg oplevede et fællesskab, jeg ikke sidenhen har prøvet, og jeg fik venskaber med mig for livet. Og så var det en stor udviklingsrejse både gennem undervisningen men lige så meget ved friheden til at rejse på egen hånd og stå på egne ben."
    />
  </div>
</section>

<!-- Statistik sektion start -->
<section
  id="statistik_sektion"
  class="maxwidthwrappper text-center w-full p-20 md:p-64"
>
  <h2 class="mb-5">ELSKET AF 2.500+ ELEVER</h2>
  <div class="grid gap-6 md:flex md:gap-10 md:mx-auto md:justify-center">
    <div class="md:max-w-xs">
      <h3 cl>16</h3>
      <p>ADVENTUREFYLDTE DESTINATIONER</p>
    </div>
    <div class="md:max-w-xs">
      <h3>4,8</h3>
      <p>PÅ TRUSTPILOT</p>
      <img class="md:max-w-xs" src="../src/_icons/5star.png" alt="" />
    </div>

    <div class="md:max-w-xs">
      <h3>106.785</h3>
      <p class="max-w-xs m-auto">
        KVADRATMETER FREDET REGNSKOV TIL BEVARELSE AF VERDENS SKOVE
      </p>
    </div>
  </div>
</section>

<!-- Statistik section  slut -->

<!-- section #2 Start -->
<style>
  section {
    overflow: hidden;
    padding-top: 5rem;
    padding-bottom: 5rem;
  }

  #section_2 {
    background-color: var(--sandbeach);
  }

  #section_2 svg {
    margin: auto;
  }

  #statistik_sektion {
    background-image: url(../src/_icons/airplane_earth.png);
    background-repeat: no-repeat;
    background-position: 50%;
    background-size: 100%;
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

  article {
    max-width: 700px;
  }
</style>
