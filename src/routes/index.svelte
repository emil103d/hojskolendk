<script>
  import OpholdCardsSection from "../components/opholdCardsSection.svelte";
</script>

<header id="video" class="relative grid grid-cols-5 mb-8">
  <video
    class="z-0 col-span-full row-span-full"
    loop
    muted
    autoplay
    src="../src/_video/herofrontpage.mp4"
  />
  <div
    class="mx-auto text-center max-w-60 z-20 col-start-2 col-end-5 row-start-1 pt-40"
  >
    <p>Rejs med HÖJSKOLENDK</p>
    <h1 class="">OG BLIV EN DEL AF FÆLLESKABET OG KOM PÅ DIT LIVS EVENTYR</h1>
  </div>
</header>

<!-- section #1 start -->
<section class="flex justify-center items-center gap-8 mt-40">
  <article class="max-w-md ml-10 md:ml-32">
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
  <img
    class=""
    src="../src/_images/forside_sektion1.png"
    alt="Unge glade mennesker der er med på et højskoleophold"
  />
</section>

<!-- section #1 slut -->
<!-- section #2 Start -->

<section id="section_2" class=" ">
  <div class="maxwidthwrappper  justify-center">
    <p class="mt-10 preh2 text-center">MANGE SPÆNDENDE DESTINATIONER</p>
    <h2 class="text-center">SE VORES EVENTYRLIGE HØJSKOLEOPHOLD</h2>
    <OpholdCardsSection />
    <button class="mx-auto">SE ALLE OPHOLD</button>
  </div>
</section>

<style>
  section {
    overflow: hidden;
  }

  #section_2 {
    background-color: var(--sandbeach);
  }
</style>
