<script>
  import SecondaryButton from "../components/secondarybutton.svelte";
  // import BuyCard from "../components/buycard.svelte";
</script>

<!-- <BuyCard /> -->

<div class="bgfooter">
  <div class="maxwidthwrapper">
    <div class="footer_kontakt">
      <div>
        <!-- hvid cirkel -->
        <div class="cirkel m-auto grid justify-center">
          <img src="src/_icons/call.png" alt="telefon ikon" />
        </div>
        <p>Ring til os</p>
      </div>
      <div>
        <!-- hvid cirkel -->
        <div>
          <div class="cirkel m-auto grid justify-center">
            <img src="src/_icons/brev.png" alt="brev ikon" />
          </div>
          <p>Skriv til os</p>
        </div>
      </div>
      <div>
        <!-- hvid cirkel -->
        <div>
          <div class="cirkel m-auto grid justify-center">
            <img src="src/_icons/messenger.png" alt="chat ikon" />
          </div>
          <p>Chat med os</p>
        </div>
      </div>
      <div>
        <!-- hvid cirkel -->
        <div>
          <div class="cirkel m-auto grid justify-center">
            <img src="src/_icons/people.png" alt="brev ikon" />
          </div>
          <p>Infomøder</p>
        </div>
      </div>
    </div>
  </div>
  <svg
    width="1728"
    height="115"
    viewBox="0 0 1728 115"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
    class="palme"
  >
    <path
      d="M427.501 61.8544C422.303 69.5676 412.501 80.3544 412.501 80.3544C380.001 81.3543 312.652 82.4144 303.5 83.3543C268 87.0002 224.5 89.1955 207 90.3543C193.687 91.2358 147.5 90.3543 112.5 95.8543C104.202 97.1583 71.5 102.319 53 105.854L0 114.354H905C902 112.07 860.5 103.834 837.5 100C814.5 96.167 664 90.3543 664 90.3543L558.5 84.3543L490.5 80.3544C473.5 79.521 437.001 76.3543 437.001 76.3543C437.001 76.3543 439.5 63.8885 442.5 52.8545C445.5 41.8205 447 35.3543 447 35.3543C448.333 35.3543 451.138 36.2989 453.5 37.8543C456 39.5002 459.167 41.8335 461.5 47.5002C463.833 53.167 465.5 69.3543 465.5 69.3543C467.5 65.3544 472.966 56.8408 474 52.8545C475 49.0002 474 40.7091 469.5 35.3543C465 29.9995 456.5 26.0187 456 25.8545C455.5 25.6903 464.7 24.2547 469.5 25.8545C475.5 27.8543 479.5 33.3544 479.5 33.3544C479.5 33.3544 480.153 24.3083 476.5 20.3205C473 16.5002 468.5 15.8548 463 15.3543C457.5 14.8538 451.5 18.3548 451.5 18.3548C450.5 15.4995 452.5 9.68111 457 7.00024C459.618 5.44044 466.784 4.59468 465.5 3.81962C460 0.500908 454.5 -1 448 3.81843C441.5 8.63686 442.5 18.3548 442.5 18.3548C438.167 16.0215 428.1 11.1548 422.501 10.3548C415.502 9.3548 414.5 9.70856 411 15.3543C407.5 21 409.167 29.0212 410.001 33.3544C411.501 30.8544 416.1 25.1546 422.501 22.3551C430.501 18.8556 437.001 27.3545 434 25.8545C431.6 24.6545 424.667 27.8192 421 30.8191C417.333 33.8191 412.001 36.8545 410.001 42.8545C408.001 48.8545 410.834 55.0212 412.501 57.3545L416.501 65.8545L422.501 52.8545C425.501 46.3545 430.501 39.3544 437.001 33.3544C442.201 28.5544 438.502 40.8882 437.001 45.3544C435.5 49.8205 431.656 55.6884 427.501 61.8544Z"
      fill="#FF5E04"
    />
  </svg>
</div>

<footer>
  <div class="footer text-center text-white">
    <img src="./src/_logo/logohvid.png" alt="logo" class="w-14 h-14" />
    <div class="footer_infomode">
      <h2 class="text-white">
        VIL DU VIDE MERE OM VORES HØJSKOLEOPHOLD I UDLANDET?
      </h2>
      <p>Tilmeld dig vores infomøder og mød nogen tidligere elever</p>

      <SecondaryButton>TILMELD INFOMØDE</SecondaryButton>
    </div>
    <div />
    <div class="footer_adress">
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

    <div class="footer_links">
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
          <li><a href="">Job hos Höjskolendk</a></li>
        </ul>
      </div>

      <ul>
        <li><strong>Læs mere her...</strong></li>
        <li><a href="">Sabbatår i udlandet</a></li>
        <li><a href="">Grupperejser for unge</a></li>
        <li><a href="">frivilligt arbejde i udlandet</a></li>
        <li><a href="">Bagpacking</a></li>
        <li><a href="">FAQ</a></li>
      </ul>
      <hr />
    </div>

    <div class="footer_some">
      <p>#hojskolen dk</p>
      <div>
        <svg
          width="202"
          height="30"
          viewBox="0 0 202 47"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect
            x="71.5"
            y="1.01514"
            width="59"
            height="44.6425"
            rx="10.5"
            stroke="white"
          />
          <path
            d="M95 35.0005V11.6721L112 23.3363L95 35.0005Z"
            stroke="white"
          />
          <path
            d="M1 19.2793H11C12.0003 16.2364 15.9009 10.1508 23.5009 10.1508C31.1009 10.1508 34.6676 16.2364 35.5009 19.2793H45.0009C45.0009 16.0674 45.0018 9.23792 45.0009 5.58652C45 2.03655 40.619 0.515137 38 0.515137H6.5C3.5 0.515137 0.999095 3.05083 1 5.07938V19.2793Z"
            stroke="white"
          />
          <path
            d="M1 23.3363H10.1466C10.1466 31.4505 15.9002 36.5219 23.5 36.5219C31.0998 36.5219 36 29.422 36 23.3363H44.9996C44.9996 27.1558 45.0005 35.2774 44.9996 39.6196C44.9987 43.8411 40.6178 45.6504 37.9989 45.6504H6.49984C3.49993 45.6504 0.999095 42.635 1 40.2226V23.3363Z"
            stroke="white"
          />
          <path
            d="M32.5 23.3364C32.5 28.6686 28.24 32.9791 23 32.9791C17.76 32.9791 13.5 28.6686 13.5 23.3364C13.5 18.0041 17.76 13.6936 23 13.6936C28.24 13.6936 32.5 18.0041 32.5 23.3364Z"
            stroke="white"
          />
          <rect
            x="34.5"
            y="4.56519"
            width="7"
            height="7.11421"
            rx="0.5"
            stroke="white"
          />
          <path
            d="M200.543 23.3364C200.543 35.681 190.89 45.6576 179.021 45.6576C167.152 45.6576 157.5 35.681 157.5 23.3364C157.5 10.9917 167.152 1.01514 179.021 1.01514C190.89 1.01514 200.543 10.9917 200.543 23.3364Z"
            stroke="white"
          />
          <path
            d="M182.372 45.1865V29.6486H187.16L188.596 22.8508H182.372C182.372 21.3941 182.372 18.3837 182.372 17.9952C182.372 17.5097 182.851 16.053 184.287 15.5674C185.436 15.179 187.638 15.4056 188.596 15.5674V9.74072C186.521 9.74072 182.181 9.74072 181.415 9.74072C179.979 9.74072 178.356 10.4785 177.106 12.1685C175.67 14.1107 175.67 16.053 175.67 17.0241V22.8508H170.404V29.6486H175.67V45.1865"
            stroke="white"
          />
        </svg>
      </div>
    </div>
  </div>
  <div class="wave">
    <svg
      width="1728"
      height="36"
      viewBox="0 0 1728 36"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M583.324 17.0145C212.805 14.4919 52.017 25.9577 0 34.8392V36L89.1389 35.4756H334.146H1728V17.0145V0C1677.8 6.83199 1524.91 26.0328 1314.9 29.3122C1052.39 33.4114 1046.47 20.1677 583.324 17.0145Z"
        fill="white"
      />
    </svg>
  </div>
  <div class="footerslut">
    <p>// HÔJSKOLENDK //</p>
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
  }

  .cirkel {
    width: 130px;
    height: 130px;
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

  footer {
    background-color: var(--orange);
    opacity: 80%;
    display: block;
    overflow: hidden;
  }

  .footer {
    color: var(--hvid);
    display: grid;
    grid-gap: 2rem;
    padding: 2rem 0;
    max-width: 1200px;
    margin: 0 auto;
  }

  footer hr {
    margin: 0 2rem;
  }

  .footerslut {
    height: 25px;
    background-color: var(--hvid);
    color: var(--textcolor);
    text-align: center;
    padding: 5px;
    font-size: 0.5rem;
  }

  .wave svg {
    max-width: 100%;
    margin-bottom: -10px;
  }

  .palme {
    margin-bottom: -1px;
    opacity: 0.8;
    overflow: inherit;
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

    footer img {
      width: 100px;
      height: 100px;
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
      padding: 7rem 0;
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

    .footer_some p {
      padding-bottom: 1.5rem;
    }
  }
  /* ----------- footer slut -------------- */
</style>
