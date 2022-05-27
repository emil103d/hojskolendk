<script>
  import SecondaryButton from "../components/secondarybutton.svelte";
  import Header from "../components/header.svelte";
</script>

<Header headerclass="src/_images/1.jpg" />

<div class="bgfooter">
  <div class="maxwidthwrapper">
    <div class="footer_kontakt">
      <div>
        <!-- hvid cirkel -->
        <div class="cirkel">
          <img src="src/_icons/call.png" alt="telefon ikon" />
        </div>
        <p>Ring til os</p>
      </div>
      <div>
        <!-- hvid cirkel -->
        <div>
          <div class="cirkel">
            <img src="src/_icons/brev.png" alt="brev ikon" />
          </div>
          <p>Skriv til os</p>
        </div>
      </div>
      <div>
        <!-- hvid cirkel -->
        <div>
          <div class="cirkel">
            <img src="src/_icons/messenger.png" alt="chat ikon" />
          </div>
          <p>Chat med os</p>
        </div>
      </div>
      <div>
        <!-- hvid cirkel -->
        <div>
          <div class="cirkel">
            <img src="src/_icons/people.png" alt="brev ikon" />
          </div>
          <p>Mød os til <br />infomøder</p>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="footerpalme">
  <svg
    width="1728"
    height="113"
    viewBox="0 0 1728 113"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M427.501 59.854C422.303 67.5672 412.501 78.354 412.501 78.354C380.001 79.354 312.652 80.414 303.5 81.3539C268 84.9999 224.5 87.1951 207 88.3539C193.687 89.2354 147.5 88.3539 112.5 93.8539C104.202 95.1579 71.5 100.319 53 103.854L0 112.354H1727.5C1727.5 112.354 1670 106.5 1665 106C1660 105.5 1622 100 1593.5 98.5C1565 97 1487 100.5 1487 100.5L1423.5 105C1423.5 105 1401.06 105.794 1380.5 106.854C1321.29 109.906 1288.27 98.3364 1229 96.8539C1145.41 94.7633 1095 105 1015 103.854C935 102.708 863 96.8539 863 96.8539L664 88.3539L558.5 82.3539L490.5 78.354C473.5 77.5206 437.001 74.3539 437.001 74.3539C437.001 74.3539 439.5 61.8881 442.5 50.8541C445.5 39.8202 447 33.3539 447 33.3539C448.333 33.3539 451.138 34.2986 453.5 35.8539C456 37.4999 459.167 39.8331 461.5 45.4999L465.5 67.3539C467.5 63.354 472.966 54.8404 474 50.8541C475 46.9999 475.5 38.9999 469.5 33.3539L456 23.8541C459.167 23.8541 464.7 22.2543 469.5 23.8541C475.5 25.8539 477 31.354 479.5 31.354C482 31.354 480.153 22.308 476.5 18.3202C473 14.4999 468.5 13.8544 463 13.3539L451.5 16.3544C452.833 14.6879 452.5 7.68074 457 4.99986C459.618 3.44007 466.98 2.06576 465.5 1.81924C459.5 0.819732 451.5 -1.71879 448 1.81805C444.5 5.35489 442.5 16.3544 442.5 16.3544C438.167 14.0211 428.1 9.15442 422.501 8.35442C415.502 7.35442 413.5 11.3539 411 13.3539C409 14.9539 409.167 27.0208 410.001 31.354C411.501 28.854 416.1 23.1542 422.501 20.3547C430.501 16.8553 437.001 25.3541 434 23.8541C431.6 22.6541 424.667 25.8188 421 28.8188C417.333 31.8187 412.001 34.8541 410.001 40.8541C408.001 46.8541 410.834 53.0208 412.501 55.3541L416.501 63.8541L422.501 50.8541C425.501 44.3541 430.501 37.354 437.001 31.354C442.201 26.554 438.502 38.8878 437.001 43.354C435.5 47.8202 431.656 53.688 427.501 59.854Z"
      fill="#FF5E04"
    />
  </svg>
</div>

<footer>
  <div class="footer text-center text-white">
    <img src="./src/_logo/logohvid.png" alt="logo" class="w-14 h-14" />
    <div class="footer_infomode">
      <h2 class="">VIL DU VIDE MERE OM VORES HØJSKOLEOPHOLD I UDLANDET?</h2>
      <p>Tilmeld dig vores infomøder og mød nogen tidligere elever</p>

      <SecondaryButton>TILMELD INFOMØDE</SecondaryButton>

      <hr class="hidden adressline2" />
    </div>
    <div />
    <div class="footer_adress">
      <div class="adressline">
        <div>
          <div>
            <ul>
              <li><strong> Adresse</strong></li>
              <li><a href="">Höjskolen DK</a></li>
              <li><a href="">Rosenørns Allé 29</a></li>
              <li><a href="">1970 Frederiksberg</a></li>
              <li><a href="">CVR: 12345678</a></li>
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
</style>
