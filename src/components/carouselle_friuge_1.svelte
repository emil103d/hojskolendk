<script>
  import Cardfri from "../components/card_friuger.svelte";
</script>

<section id="section_2">
  <div id="carowrapper">
    <button id="left" class="hover:scale-105 hidden md:absolute"
      ><svg
        width="42"
        height="66"
        viewBox="0 0 42 66"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M39.4561 62.7832L4.78214 31.6962L39.4561 3.0006"
          stroke="black"
          stroke-width="6"
        />
      </svg>
    </button>

    <div class="flex gap-5 overflow-x-scroll object-cover">
      <Cardfri
        image="../src/_images/friuge_1.jpg"
        title="Uge på Mahfushi"
        addon="ADD ON"
        text="Tag på udflugt til Mahfushi et af verdens bedste surfsteder, så i skal selføgelig lærer at “ride the waves”.  
        Hawaii er et af verdens bedste surfstede af, så i skal så i skal selføgelig lærer at “ride the waves”.  
        "
        class="object-cover"
      />
      <Cardfri
        image="../src/_images/webp/m_yoga.webp"
        title="Yoga på stranden"
        addon="INKLUDED"
        text="Yoga på stranden er fantastisk afbræk så i skal selføgelig lærer at “ride the waves”.  
        Hawaii er et af verdens bedste surfsteder, så i.Hawaii er et af verdens bedste surfsteder, så i skal selføgelig lærer at “ride the waves”.  
        "
      />
      <Cardfri
        image="../src/_images/webp/m_nightf.webp"
        title="Night fishing trip"
        addon="ADD ON"
        text="Tag ud om natten og fang fisk med line, , så i skal selføgelig lærer at “ride the waves”.  
        Hawaii er et af verdens bedste surfsteder, så i.Hawaii er et af verdens bedste surfsteder, så i skal selføgelig lærer at “ride the waves”.  
        "
      />
      <Cardfri
        image="../src/_images/webp/m_hest.webp"
        title="Ridetur på øen"
        addon="ADD ON"
        text="En unik måde at se øen på fire ben så i skal selføgelig lærer at “ride the waves”.  
        Hawaii er et af verdens bedste surfsteder er et af verdens bedste surfsteder, så i skal selføgelig lærer at “ride the waves”.  
        "
      />

      <Cardfri
        image="../src/_images/webp/m_hotel.webp"
        title="Dagstur til Hilton hotelø"
        addon="ADD ON"
        text="Trænger du til luksus?il Hilton hotel så i skal selføgelig lærer at “ride the waves”.  
        Hawaii er et af verdens bedste surfsteder, så i.Hawaii er et af verdens bedste surfsteder, så i skal selføgelig lærer at “ride the waves”.  
        "
      />

      <Cardfri
        image="../src/_images/webp/m_snorkel.webp"
        title="Snorkling"
        addon="ADD ON"
        text="Et af verdens smukkeste steder at snorkle,  så i skal selføgelig lærer at “ride the waves”.  
        Hawaii er et af verdens bedste surfsteder, så i.Hawaii er et af verdens bedste surfsteder, så i skal selføgelig lærer at “ride the waves”.  
        "
      />
    </div>
    <button id="right" class="hover:scale-105 hidden md:absolute"
      ><svg
        width="43"
        height="66"
        viewBox="0 0 43 66"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M2.95605 2.92773L37.8401 34.2031L2.95605 63.0727"
          stroke="black"
          stroke-width="6"
        />
      </svg>
    </button>
  </div>
</section>

<style>
  #section_2 {
    justify-content: center;
    margin-left: auto;
    margin-right: auto;
    overflow: hidden;
    max-width: 100%;
  }

  #carowrapper {
    position: relative;
    overflow: hidden;
  }

  button {
    transition: transform 0.2s;
  }

  #left svg {
    height: 20px;
    width: 20px;
    margin-left: auto;
    margin-right: auto;
  }

  #right svg {
    height: 20px;
    width: 20px;
    margin-left: auto;
    margin-right: auto;
  }

  #left {
    background-color: white;
    border-radius: 50px;
    height: 40px;
    width: 40px;
    top: 40%;
    left: 0;
    position: absolute;
    z-index: 10;
  }

  #right {
    background-color: white;
    border-radius: 50px;
    height: 40px;
    width: 40px;
    top: 40%;
    right: 0;
    position: absolute;
    z-index: 10;
  }
</style>
