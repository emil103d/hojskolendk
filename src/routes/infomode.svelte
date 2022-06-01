<script>
  import Header from "../components/header.svelte";
  import Infomodecard from "../components/infomode_card.svelte";
</script>

<Header
  imgtitle="src/_images/webp/social7.webp"
  subtitle="Få svar på alle dine spørgsål"
  title="VÆR MED TIL VORES INFOMØDER"
/>
<main>
  <div class="preh2">
    <a href="indec">FORSIDE /</a>
    <a href="alleophold" class="underline preh2">TILMELD INFOMODE</a>
  </div>

  <section class="maxwidthwrapper">
    <p class="preh2">Gratis & uforpligtende</p>
    <h2>INFOMØDER 6 REJSEFEBER CAFÉ</h2>
    <p>
      Hør meget mere om vores højskoleophold i udllandet og møde nogle af vores
      skønne tidligere elever til en aften med billeder, historier og gode
      vibes.
    </p>
    <br>
    <hr>
  </section>

  <section class="maxwidthwrapper grid gap-10">
    <h3>Maj 2022</h3>
    <Infomodecard
      image="src/_images/webp/social7.webp"
      title="Infomøde København"
      subtitle="For dig der drømmer om dit livs eventyr"
      dato="06 Maj 22"
      tid="Kl. 17:00 - 19:00"
      adresse="Studenterhuset København
Købmagergade 29,
1970 Købbenhavn K"
    />
    <Infomodecard
      image="src/_images/webp/social7.webp"
      title="Infomøde Aarhus"
      subtitle="For dig der drømmer om dit livs eventyr"
      dato="10 Maj 22"
      tid="Kl. 17:00 - 19:00"
      adresse="Studenterhuset Aarhus
Købmagergade 29,
1970 Aarhus"
    />
    <Infomodecard
      image="src/_images/webp/social7.webp"
      title="Online Infomøde"
      subtitle="For dig der drømmer om dit livs eventyr"
      dato="12 Maj 22"
      tid="Kl. 17:00 - 19:00"
      adresse="Zoom.com"
    />
  </section>

  <section class="maxwidthwrapper grid">
    <h3>Juni 2022</h3>
    <Infomodecard
      image="src/_images/webp/social7.webp"
      title="Infomøde Online"
      subtitle="For dig der drømmer om dit livs eventyr"
      dato="06 Maj 22"
      tid="Kl. 17:00 - 19:00"
      adresse="Zoom"
    />
  </section>
</main>

<style>
  main {
    background-image: url(src/_icons/gurfers.png);
    background-position: cover;
    background-size: 200%;
    background-repeat: repeat-y;
    background-position-x: 10%;
  }

  section {
    padding-top: var(--padding-sections);
    padding-bottom: var(--padding-sections);
  }
</style>
