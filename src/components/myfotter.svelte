<script>
  import MyButton from "../components/button.svelte";
  // import BuyCard from "../components/buycard.svelte";
</script>

<!-- <BuyCard /> -->

<div class="bgfooter overflow-hidden">
  <div class="maxwidthwrapper">
    <div class="footer_kontakt">
      <div>
        <!-- hvid cirkel -->
        <div class="cirkel m-auto grid justify-center">
          <img class="m-auto" src="call.png" alt="telefon ikon" />
        </div>
        <p>Ring til os</p>
      </div>
      <div>
        <!-- hvid cirkel -->
        <div>
          <div class="cirkel m-auto grid justify-center">
            <img class="m-auto" src="brev.png" alt="brev ikon" />
          </div>
          <p>Skriv til os</p>
        </div>
      </div>
      <div>
        <!-- hvid cirkel -->
        <div>
          <div class="cirkel m-auto grid justify-center">
            <img class="m-auto" src="messenger.png" alt="chat ikon" />
          </div>
          <p>Chat med os</p>
        </div>
      </div>
      <div>
        <!-- hvid cirkel -->
        <div>
          <div class="cirkel m-auto grid justify-center">
            <img class="m-auto" src="people.png" alt="brev ikon" />
          </div>
          <p>Infomøder</p>
        </div>
      </div>
    </div>
  </div>

  <div class="palme overflow-hidden">
    <svg
      width="1725"
      height="114"
      viewBox="0 0 1725 114"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M427.501 61.1123C422.303 68.8256 412.501 79.6124 412.501 79.6124C380.001 80.6123 312.652 81.6723 303.5 82.6123C268 86.2582 224.5 88.4535 207 89.6123C193.687 90.4938 147.5 89.6123 112.5 95.1123C104.202 96.4163 71.5 101.577 53 105.112L0 113.612H1724.5C1721.5 111.328 1399 95.1123 1399 95.1123L664 89.6123L558.5 83.6123L490.5 79.6124C473.5 78.779 437.001 75.6123 437.001 75.6123C437.001 75.6123 439.5 63.1464 442.5 52.1125C445.5 41.0785 447 34.6123 447 34.6123C448.333 34.6123 451.138 35.5569 453.5 37.1123C456 38.7582 459.167 41.0915 461.5 46.7582C463.833 52.4249 465.5 68.6123 465.5 68.6123C467.5 64.6123 472.966 56.0987 474 52.1125C475 48.2582 474 39.9671 469.5 34.6123C465 29.2575 456.5 25.2767 456 25.1125C455.5 24.9483 464.7 23.5126 469.5 25.1125C475.5 27.1123 479.5 32.6123 479.5 32.6123C479.5 32.6123 480.153 23.5663 476.5 19.5785C473 15.7582 468.5 15.1128 463 14.6123C457.5 14.1117 451.5 17.6128 451.5 17.6128C450.5 14.7575 452.5 8.93909 457 6.25821C459.618 4.69842 466.784 3.85265 465.5 3.07759C460 -0.241119 454.5 -1.74203 448 3.0764C441.5 7.89483 442.5 17.6128 442.5 17.6128C438.167 15.2794 428.1 10.4128 422.501 9.61277C415.502 8.61277 414.5 8.96654 411 14.6123C407.5 20.258 409.167 28.2792 410.001 32.6123C411.501 30.1124 416.1 24.4126 422.501 21.613C430.501 18.1136 437.001 26.6125 434 25.1125C431.6 23.9125 424.667 27.0771 421 30.0771C417.333 33.0771 412.001 36.1125 410.001 42.1125C408.001 48.1125 410.834 54.2791 412.501 56.6125L416.501 65.1125L422.501 52.1125C425.501 45.6125 430.501 38.6123 437.001 32.6123C442.201 27.8123 438.502 40.1462 437.001 44.6123C435.5 49.0785 431.656 54.9463 427.501 61.1123Z"
        fill="#FF5E04"
      />
    </svg>
  </div>
</div>

<footer class="">
  <div class="footer text-center py-4 mb-30">
    <img src="logohvid.png" alt="logo" class="w-14 h-14" />
    <div class="footer_infomode ">
      <h2 class="text-white">
        VIL DU VIDE MERE OM VORES HØJSKOLEOPHOLD I UDLANDET?
      </h2>
      <p class="text-white mb-4">Tilmeld dig et infomøde og hør meget mere..</p>

      <MyButton type="secondary">TILMELD INFOMØDE</MyButton>
    </div>
    <div />
    <div class="footer_adress text-white">
      <div class="adressline">
        <div>
          <div>
            <ul>
              <li><strong> Adresse</strong></li>
              <li>HÔJSKOLENDK</li>
              <li>Rosenørns Allé 29</li>
              <li>1970 Frederiksberg</li>
              <li>CVR: 12345678</li>
            </ul>
            <br />
          </div>

          <div>
            <ul>
              <li><strong>Kontakt info</strong></li>
              <li>+45 3967 2065</li>
              <li><a href="">info@hojskolen.dk</a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>

    <div class="footer_links text-white">
      <div>
        <ul>
          <li><strong> Samarbejdspartnere</strong></li>
          <li><a href="">Jysk Rejsebureau</a></li>
          <li><a href="">Gauda Rejseforsikring</a></li>
          <li><a href="">Lokale partnere</a></li>
          <li><a href="">Trees.org</a></li>
          <li><a href="">Trees for the future</a></li>
          <li><a href="">River Online</a></li>
          <li><a href="">World Animal Protection</a></li>
        </ul>
      </div>

      <div>
        <ul>
          <li><strong> Praktiske informationer</strong></li>
          <li><a href="">Cookiepolitik</a></li>
          <li><a href="">Privatlivspolitik</a></li>
          <li><a href="">Handelsbetingelser</a></li>
          <li><a href="">Fortrydelsesret</a></li>
          <li><a href="">Rejsegarantifonden</a></li>
          <li><a href="">Covid-19 informationer</a></li>
          <li><a href="">Job hos HÔJSKOLENDK</a></li>
        </ul>
      </div>

      <ul>
        <li><strong>Læs mere her...</strong></li>
        <li><a href="">Sabbatår i udlandet</a></li>
        <li><a href="">Grupperejser for unge</a></li>
        <li><a href="">Frivilligt arbejde i udlandet</a></li>
        <li><a href="">Backpacking</a></li>
        <li><a href="">FAQ</a></li>
      </ul>
      <hr />
    </div>

    <div class="footer_some">
      <p class="text-white">#hojskolendk</p>
      <div class="footer_ikons">
        <a href="https://www.facebook.com/hojskolendk/"
          ><img src="facebook.png" alt="Facebook Link" /></a
        >
        <a href="https://www.instagram.com/hojskolendk/?hl=da"
          ><img src="instagram.png" alt="Instagram Link" /></a
        >
        <a href="https://www.youtube.com/c/HojskolendkDk"
          ><img src="youtube.png" alt="Youtube Link" /></a
        >
      </div>
    </div>
  </div>

  <div class="wave">
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
  <div id="footerslut">
    <p class="text-black">// HÔJSKOLENDK //</p>
  </div>
</footer>

<style>
  /* ---------------Footer start  -----------------*/

  footer p,
  footer a,
  footer li {
    font-size: 0.8rem;
    font-weight: 200;
    text-decoration: none;
  }

  a:hover {
    text-decoration: underline;
  }

  .footer_kontakt {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 1rem;
    text-align: center;
    padding-bottom: 4rem;
  }

  .footer_links {
    display: grid;
    gap: 1.5rem;
  }

  .bgfooter {
    background-color: var(--sandbeach);
    padding-top: 5rem;
  }

  .cirkel {
    width: 120px;
    height: 120px;
    background-color: white;
    border-radius: 100px;
    margin: auto;
  }

  footer img {
    margin: auto;
  }

  .footer_kontakt img {
    width: 60px;
    height: 60px;
  }

  .footer_some img {
    width: 30px;
    height: 30px;
  }

  .footer_some {
    display: grid;
    grid-template-rows: auto auto;
    margin: auto;
  }

  .footer_ikons {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 15px;
  }

  footer {
    background-color: var(--orange);
    opacity: 80%;
    display: block;
    overflow: hidden;
  }

  .footer {
    display: grid;
    grid-gap: 2rem;
    padding: 2rem 0;
    max-width: 1400px;
    margin: 0 auto;
  }

  footer hr {
    margin: 0 2rem;
  }

  #footerslut {
    height: 25px;
    background-color: var(--hvid);
    color: var(--textcolor);
    text-align: center;
    padding: 5px;
    font-size: 0.5rem;
    padding-top: 60px;
    padding-bottom: 60px;
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

  .palme {
    margin-bottom: -0.9px;
    opacity: 0.8;
    overflow: hidden;
    width: 100vw;
  }
  /* ---------------Footer slut */

  /* ----------- footer start -------------- */
  @media screen and (min-width: 700px) {
    footer,
    footer p,
    footer a,
    footer li {
      font-size: 0.7rem;
      font-weight: 400;
    }
    footer h2 {
      font-size: 0.9rem;
      padding-top: 3.5rem;
      padding-bottom: 1rem;
    }

    .cirkel {
      width: 180px;
      height: 180px;
      background-color: white;
      border-radius: 100px;
      margin: auto;
    }

    .palme {
      overflow: hidden;
      width: 100vw;
    }

    footer img {
      width: 84px;
      height: 84px;
      margin: 0;
      margin-bottom: -16px;
      margin-top: 15px;
    }

    .footerline {
      width: 1px;
      background-color: var(--hvid);
      opacity: 50%;
    }

    .footer_kontakt {
      grid-template-columns: 1fr 1fr 1fr 1fr;
    }
    .footer_kontakt img {
      margin: auto;
    }

    .footerline1 {
      display: block;
    }

    .footer {
      display: grid;
      grid-template-columns: 1fr 3fr 1fr;
      grid-template-rows: auto auto auto;
      font-size: 0.8rem;
      padding: 0 2rem;
      margin-bottom: 5rem;
    }

    .footer_adress {
      grid-column: 1/2;
      grid-row: 2/4;
      text-align: left;
    }

    .footer_links {
      display: flex;
      justify-content: space-between;
      text-align: left;
      line-height: 1.9;
      grid-row: 2/4;
    }

    .footer_infomode {
      grid-column: 3/4;
      grid-row: 1/3;
    }

    .footer_some {
      grid-column: 3/4;
      grid-row: 3/4;
    }

    .footer_some svg {
      margin: auto 0;
    }
  }
  /* ----------- footer slut -------------- */
</style>
