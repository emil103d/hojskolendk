<script>
  import Header from "../components/header.svelte";
  import Infomodecard from "../components/infomode_card.svelte";
</script>

<Header
  imgtitle="social7.webp"
  subtitle="Få svar på alle dine spørgsål"
  title="VÆR MED TIL VORES INFOMØDER"
/>
<main>
  <div class="preh2">
    <a href="indec">Forside /</a>
    <a href="alleophold" class="underline preh2">Tilmeld infomøde</a>
  </div>

  <section class="maxwidthwrapper">
    <p class="preh2">GRATIS & UFORPLIGTENDE</p>
    <h2>INFOMØDER & REJSEFEBER CAFÉ</h2>
    <p>
      Hør meget mere om vores højskoleophold i udlandet og møde nogle af vores
      skønne tidligere elever til en aften med billeder, historier og gode
      vibes. Vi fortæller meget mere om de rejseeventyr som venter!
    </p>
    <br />
    <hr />
  </section>

  <section class="maxwidthwrapper grid gap-10">
    <h3>Maj 2022</h3>
    <Infomodecard
      image="stud_kbh.webp"
      title="Infomøde København"
      subtitle="For dig der drømmer om dit livs eventyr"
      dato="06 Maj 22"
      tid="Kl. 17:00 - 19:00"
      adresse="Studenterhuset København Købmagergade 29, 1970 Købbenhavn K"
    />
    <Infomodecard
      image="stud_odense.webp"
      title="Infomøde Odense"
      subtitle="For dig der drømmer om dit livs eventyr"
      dato="10 Maj 22"
      tid="Kl. 17:00 - 19:00"
      adresse="Studenterhuset Aarhus
Købmagergade 29,
1970 Aarhus"
    />
    <Infomodecard
      image="zoom.webp"
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
      image="stud_kbh.webp"
      title="Infomøde København"
      subtitle="For dig der drømmer om dit livs eventyr"
      dato="06 Juni 22"
      tid="Kl. 17:00 - 19:00"
      adresse="Studenterhuset København Købmagergade 29, 1970 Købbenhavn K"
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
