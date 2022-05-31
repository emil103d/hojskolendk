<script>
  import CardTrustpilot from "../components/card_trustpilot.svelte";
  import Card from "../components/card.svelte";
  import PrimaryButton from "../components/primarybutton.svelte";
  import Cookie from "../components/cookie.svelte";
  import Chat from "../components/chat.svelte";
  import Saos from "saos";
  let cookie;
</script>

<header class="h-full w-full" id="video">
  <video
    class="z-0 hero-image"
    loop
    muted
    autoplay
    src="../src/_video/herofrontpage.mp4"
  />
  <div class="hero-text m-auto">
    <p>HØJSKOLEOPHOLD I UDLANDET</p>
    <h1 class="">FÆLLESKAB & REJSEEVENTYR</h1>
  </div>
</header>

<!-- section #1 start -->
<section
  class="maxwidthwrapper md:pt-0 md:grid grid-cols-2 md:justify-center md:gap-8"
>
  <Saos animation={"from-left 2s cubic-bezier(0.35, 0.5, 0.65, 0.95) both"}>
    <article class="cols-start-1 grid items-center">
      <div>
        <p class="preh2">VI ER</p>
        <h2>REJSEEVENTYR, SOMMER VIBES & ET FÆLLESSKAB I VERDENSKLASSE</h2>
        <p>
          HÖJSKOLENDK er noget for dig, hvis du vil på højskole i udlandet og er
          vild med højskolefællesskab, vil med på et fantastisk rejseeventyr,
          glæder dig til at lære om fremmede kulturer, vil rejse med rygsæk,
          drømmer om en fed grupperejse med andre skønne unge, vil opleve et
          stærkt sammenhold og ønsker inspirerende og meningsfuld undervisning.
          Du er sikker på en tryg rejseoplevelse da vi er medlem af
          Rejsegarantifonden.
        </p>
        <button>JOIN OS TIL INFOMØDE</button>
      </div>
    </article>
  </Saos>
  <div class="cols-start-2">
    <Saos
      animation={"slide-in-fwd-tr 0.5s cubic-bezier(0.250, 0.460, 0.450, 0.940) both"}
      animation_out={"scale-out-center 0.5s cubic-bezier(0.550, 0.085, 0.680, 0.530) both"}
      top={250}
      bottom={250}
    >
      <img
        class=""
        src="../src/_images/webp/sektion1.webp"
        alt="Unge glade mennesker der er med på et højskoleophold"
      />
    </Saos>
  </div>
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
      <Card
        image="../src/_images/webp/ophold4.webp"
        title="Costa Rica, Mexico & Guatemala"
      />
    </div>
    <div class="md:justify-center md:grid">
      <PrimaryButton class="primarybutton"
        >UDFORSK ALLE VORES OPHOLD</PrimaryButton
      >
    </div>

  </div>
</section>

<!-- section #2 Start -->
<section class="maxwidthwrapper mx-auto pb-0">
  <div class="">
    <p class="preh2">ELSKET AF 2500+ ELEVER</p>
    <h2>SE VORES ANMELDELSER</h2>
    <img src="../src/_logo/trustpilot_logo.png" alt="" />
    <div class="md:flex grid gap-16 md:gap-5 mt-10 mx-auto justify-around">
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
  id="statistik_sektion"
  class="maxwidthwrapper text-center w-full md:p-64 min-h-[35vh] grid items-center justify-center"
>
  <div class="">
    <h2 class="mb-5 hidden">ELSKET AF 2.500+ ELEVER</h2>

    <div class="grid gap-6 md:flex md:gap-40 md:mx-auto md:justify-center">
      <div class="md:max-w-xs">
        <h3 cl>16</h3>
        <p>ADVENTUREFYLDTE <br /> DESTINATIONER</p>
      </div>

      <div class="md:max-w-xs">
        <h3>4,8</h3>
        <p>PÅ TRUSTPILOT</p>
        <img class="md:max-w-xs" src="../src/_icons/5star.png" alt="" />
      </div>

      <div class="md:max-w-xs">
        <h3>106.785</h3>
        <p class="max-w-xs m-auto">M2 FREDET REGNSKOV</p>
      </div>
    </div>
  </div>
</section>

<section class="maxwidthwrapper">
  <p class="preh2">WE'RE SOCIAL</p>
  <h2>FØLG VORES REJSEEVENTYR @ HÖJSKOLENDK</h2>
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

  #section_2 svg {
    margin: auto;
  }

  #statistik_sektion {
    background-image: url(../src/_icons/airplane_earth.png);
    background-size: cover;
    background-position: 50%;
    background-repeat: no-repeat;
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
