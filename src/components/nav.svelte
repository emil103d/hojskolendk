<script>
  import { onMount } from "svelte";

  // Show mobile icon and display menu
  let showMobileMenu = false;

  // Mobile menu click event handler
  const handleMobileIconClick = () => (showMobileMenu = !showMobileMenu);

  // Media match query handler
  const mediaQueryHandler = (e) => {
    // Reset mobile state
    if (!e.matches) {
      showMobileMenu = false;
    }
  };

  // Attach media query listener on mount hook
  onMount(() => {
    const mediaListener = window.matchMedia("(max-width: 800px)");

    mediaListener.addListener(mediaQueryHandler);
  });
</script>

<nav class="w-screen flex md:grid md:grid-cols-3">
  <a sveltekit:prefetch href="/">
    <img class="" src="../src/_logo/logohvid.png" alt="logo hvid" /></a
  >

  <div class="inner  justify-end ">
    <div
      on:click={handleMobileIconClick}
      class={`mobile-icon${showMobileMenu ? " active" : ""}`}
    >
      <div class="middle-line" />
    </div>
    <ul class={`navbar-list${showMobileMenu ? " mobile" : ""}`}>
      <li id="" class="bg-black lg:hidden">
        <div
          class="accordion flex-col flex overflow-scroll max-h-[90vh] flex-nowrap"
        >
          <!--  Panel 1  -->
          <div class="">
            <input type="checkbox" name="panel" id="panel-1" class="hidden" />
            <p
              for="panel-1"
              class="relative block bg-black text-white p-4 shadow border-b border-grey"
            >
              <a href="/alleophold">Se alle ophold</a>
            </p>
          </div>
          <!--  Panel 2  -->
          <div class="">
            <input type="checkbox" name="panel" id="panel-2" class="hidden" />
            <label
              for="panel-2"
              class="relative block bg-black text-white p-4 shadow border-b border-grey"
              >Højskoleophold 5 Uger</label
            >
            <div class="accordion__content overflow-hidden bg-grey-lighter">
              <ul class="accordion__body p-4" id="panel1">
                <li class="text-white">
                  <a href="/singlepage">BALI, LOMBOK & GILI ISLANDS</a>
                </li>
                <li class="text-white">
                  <a href="/singlepage">NEW YORK CITY & CARIBIEN</a>
                </li>
              </ul>
            </div>
          </div>
          <!-- Panel 3 -->
          <div class="">
            <input type="checkbox" name="panel" id="panel-3" class="hidden" />
            <label
              for="panel-3"
              class="relative block bg-black text-white p-4 shadow border-b border-grey"
              >2 Måneder</label
            >
            <div class="accordion__content overflow-hidden bg-grey-lighter">
              <ul class="accordion__body p-4" id="panel1">
                <li class="text-white">
                  <a href="/singlepage"
                    >Maldiverne, Sri Lanka, Bali & Gili Islands</a
                  >
                </li>
                <li class="text-white">
                  <a href="/singlepage"
                    >Hawaii, Australien, Japan, Bali & Gili Islands</a
                  >
                </li>
              </ul>
            </div>
          </div>
          <!--  Panel 4  -->
          <div class="">
            <input type="checkbox" name="panel" id="panel-4" class="hidden" />
            <label
              for="panel-4"
              class="relative block bg-black text-white p-4 shadow border-b border-grey"
              >3 Måneder</label
            >
            <div class="accordion__content overflow-hidden bg-grey-lighter">
              <ul class="accordion__body p-4" id="panel1">
                <li class="text-white">
                  <a href="/singlepage">CARIBIEN, HAWAII & MEXICO</a>
                </li>
                <li class="text-white">
                  <a href="/singlepage">Indien, Nepal, Thailand & Sri Lanka</a>
                </li>
                <li class="text-white">
                  <a href="/singlepage">COSTA RICA, MEXICO & GUATEMALA</a>
                </li>
              </ul>
            </div>
          </div>

          <!--  Panel 5  -->
          <div class="">
            <input type="checkbox" name="panel" id="panel-5" class="hidden" />
            <p
              for="panel-5"
              class="relative block bg-black text-white p-4 shadow border-b border-grey"
            >
              <a href="/infomode">Infomøder</a>
            </p>
          </div>

          <!--  Panel 6  -->
          <div class="">
            <input type="checkbox" name="panel" id="panel-6" class="hidden" />
            <label
              for="panel-6"
              class="relative block bg-black text-white p-4 shadow border-b border-grey"
              >Om os</label
            >
            <div class="accordion__content overflow-hidden bg-grey-lighter">
              <ul class="accordion__body p-4" id="panel1">
                <li class="text-white">
                  <a href="/underconstruction">Mød teamet</a>
                </li>
                <li class="text-white">
                  <a href="/underconstruction">Vores Værdier</a>
                </li>
                <li class="text-white">
                  <a href="/underconstruction">Bæredygtighed</a>
                </li>
                <li class="text-white">
                  <a href="/underconstruction">FAQ</a>
                </li>
                <li class="text-white">
                  <a href="/underconstruction">Blog</a>
                </li>

                <li class="text-white">
                  <a href="/underconstruction">Det siger vores elever</a>
                </li>
              </ul>
            </div>
          </div>
          <!--  Panel 7  -->
          <div class="">
            <input type="checkbox" name="panel" id="panel-7" class="hidden" />
            <label
              for="panel-7"
              class="relative block bg-black text-white p-4 shadow border-b border-grey"
              >Elevforening</label
            >
            <div class="accordion__content overflow-hidden ">
              <ul class="accordion__body p-4" id="panel1">
                <li class="text-white">
                  <a href="/underconstruction">Kommende Events</a>
                </li>
                <li class="text-white">
                  <a href="/underconstruction">Elev Ambasadører</a>
                </li>
                <li class="text-white">
                  <a href="/underconstruction">REUNION</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </li>

      <li class="hidden lg:block">
        <div class="group relative h-full">
          <a
            href="/alleophold"
            class="text-white flex items-center h-full bg-grey-darkest px-4"
          >
            Højskoleophold
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              width="24"
              height="24"
              class="h-6 w-6 text-grey-darker fill-current ml-1"
              ><path
                class="heroicon-ui"
                d="M15.3 9.3a1 1 0 0 1 1.4 1.4l-4 4a1 1 0 0 1-1.4 0l-4-4a1 1 0 0 1 1.4-1.4l3.3 3.29 3.3-3.3z"
              /></svg
            >
          </a>
          <div
            id="hover_underkategori"
            class="hidden p-4 pb-6 group-hover:grid absolute pin-r top-full grid-cols-3 grid-rows-2 bg-black -left-full"
          >
            <div id="hover_underkategori" class="col-span-3 flex items-center">
              <img class="ikoner" src="../src/_icons/flyafgang.png" alt="" />

              <a
                href="/alleophold"
                id="topnav_titel"
                class="block text-left py-3 px-3 text-white"
              >
                Se alle ophold
              </a>
            </div>

            <div class="columns-1 block">
              <div class="flex items-center">
                <img class="ikoner" src="../src/_icons/flyafgang.png" alt="" />

                <p class="text-white">5 uger</p>
              </div>
              <ul class="block">
                <li class="text-white flex items-center">
                  <svg
                    class=" ml-4"
                    width="10"
                    height="10"
                    viewBox="0 0 10 10"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <circle cx="5" cy="5" r="5" fill="white" />
                  </svg>
                  <a href="/singlepage">Bali, Lombok & Gili Islands</a>
                </li>
                <li class="text-white flex items-center">
                  <svg
                    class=" ml-4"
                    width="10"
                    height="10"
                    viewBox="0 0 10 10"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <circle cx="5" cy="5" r="5" fill="white" />
                  </svg>
                  <a href="/singlepage">Indien, Nepal, Thailand & Sri Lanka</a>
                </li>
              </ul>
            </div>
            <div class="columns-1 block justify-start">
              <div class="flex items-center">
                <img class="ikoner" src="../src/_icons/flyafgang.png" alt="" />

                <p class="text-white">2 måneders ophold</p>
              </div>
              <ul class="block">
                <li class="text-white flex items-center">
                  <svg
                    class=" ml-4"
                    width="10"
                    height="10"
                    viewBox="0 0 10 10"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <circle cx="5" cy="5" r="5" fill="white" />
                  </svg>
                  <a href="/singlepage"
                    >Maldiverne, Sri Lanka, Bali & Gili Islands</a
                  >
                </li>
                <li class="text-white flex items-center">
                  <svg
                    class=" ml-4"
                    width="10"
                    height="10"
                    viewBox="0 0 10 10"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <circle cx="5" cy="5" r="5" fill="white" />
                  </svg>
                  <a href="/singlepage">xxx</a>
                </li>
              </ul>
            </div>
            <div class="columns-1 block">
              <div class="flex items-center">
                <img class="ikoner" src="../src/_icons/flyafgang.png" alt="" />

                <p class="text-white">3 måneders ophold</p>
              </div>
              <ul class="block">
                <li class="text-white flex items-center">
                  <svg
                    class=" ml-4"
                    width="10"
                    height="10"
                    viewBox="0 0 10 10"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <circle cx="5" cy="5" r="5" fill="white" />
                  </svg>
                  <a href="/singlepage">Costa Rica, Mexico & Guatemala</a>
                </li>
                <li class="text-white flex items-center">
                  <svg
                    class=" ml-4"
                    width="10"
                    height="10"
                    viewBox="0 0 10 10"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <circle cx="5" cy="5" r="5" fill="white" />
                  </svg>
                  <a href="/singlepage">Indien, Nepal, Thailand & Sri Lanka</a>
                </li>
                <li class="text-white flex items-center">
                  <svg
                    class=" ml-4"
                    width="10"
                    height="10"
                    viewBox="0 0 10 10"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <circle cx="5" cy="5" r="5" fill="white" />
                  </svg>
                  <a href="/singlepage"
                    >Hawaii, Australien, Japan, Bali & Gili Islands</a
                  >
                </li>
                <li class="text-white flex items-center">
                  <svg
                    class=" ml-4"
                    width="10"
                    height="10"
                    viewBox="0 0 10 10"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <circle cx="5" cy="5" r="5" fill="white" />
                  </svg>
                  <a href="/singlepage">Caribien, Hawaii & Mexico</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </li>
      <li class="hidden lg:block">
        <div class="group relative h-full">
          <a
            href="/infomode"
            class="text-white flex items-center h-full bg-grey-darkest px-4"
          >
            Infomøder
          </a>
        </div>
      </li>
      <li class="hidden lg:block">
        <div class="group relative h-full">
          <a
            href="/underconstruction"
            class="text-white flex items-center h-full bg-grey-darkest px-4"
          >
            Om os
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              width="24"
              height="24"
              class="h-6 w-6 text-grey-darker fill-current ml-1"
              ><path
                class="heroicon-ui"
                d="M15.3 9.3a1 1 0 0 1 1.4 1.4l-4 4a1 1 0 0 1-1.4 0l-4-4a1 1 0 0 1 1.4-1.4l3.3 3.29 3.3-3.3z"
              /></svg
            >
          </a>
          <div
            class="hidden group-hover:block absolute pin-r top-full w-48 bg-black"
          >
            <ul>
              <li>
                <a
                  href="/underconstruction"
                  class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
                >
                  Møde teamet
                </a>
              </li>
              <li>
                <a
                  href="/underconstruction"
                  class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
                >
                  Vores værdier
                </a>
              </li>
              <li>
                <a
                  href="/underconstruction"
                  class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
                >
                  Bæredygtighed
                </a>
              </li>
              <li>
                <a
                  href="/underconstruction"
                  class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
                >
                  FAQ
                </a>
              </li>
              <li>
                <a
                  href="/underconstruction"
                  class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
                >
                  Blog
                </a>
              </li>
              <li>
                <a
                  href="/underconstruction"
                  class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
                >
                  Det siger vores elever
                </a>
              </li>
            </ul>
            <div class="footer_some mr-3 mb-6">
              <div class="h-0.5 mt-2 w-48 bg-gray-800 pr-12" />
              <div class="mt-5">
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
        </div>
      </li>
      <li class="hidden lg:block">
        <div class="group relative h-full">
          <a
            href="/underconstruction"
            class="text-white flex items-center h-full bg-grey-darkest px-4"
          >
            Elevforening
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              width="24"
              height="24"
              class="h-6 w-6 text-grey-darker fill-current ml-1"
              ><path
                class="heroicon-ui"
                d="M15.3 9.3a1 1 0 0 1 1.4 1.4l-4 4a1 1 0 0 1-1.4 0l-4-4a1 1 0 0 1 1.4-1.4l3.3 3.29 3.3-3.3z"
              /></svg
            >
          </a>
          <div
            class="hidden group-hover:block absolute pin-r top-full w-48 bg-black"
          >
            <ul>
              <li>
                <a
                  href="/underconstruction"
                  class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
                >
                  Kommende Events
                </a>
              </li>
              <li>
                <a
                  href="/underconstruction"
                  class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
                >
                  Elev Ambassadøre
                </a>
              </li>
              <li>
                <a
                  href="/underconstruction"
                  class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
                >
                  REUIONEN 2022
                </a>
              </li>
            </ul>
          </div>
        </div>
      </li>
    </ul>
    <button class="hidden lg:block"
      ><a href="/infomode">TILMELD INFOMØDE</a></button
    >
  </div>
</nav>

<!------------------- Credits   ---------------------->

<!-- https://linguinecode.com/post/create-a-navbar-in-svelte -->
<style>
  nav {
    background: #000000;
    opacity: 0.9;
    height: 100px;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 2000;
  }

  #mobile_position {
    position: fixed;
  }
  img {
    width: 4rem;
    margin: 1rem;
    z-index: 30;
    align-self: center;
  }

  .ikoner {
    width: 2rem;
    margin: 1rem;
  }
  .inner {
    max-width: 900px;
    padding-left: 20px;
    margin: auto;
    box-sizing: border-box;
    display: flex;
    align-items: center;
    height: 100%;
    width: 65vw;
  }

  button {
    font-family: "Lato", sans-serif;
    background-color: var(--primary-button-cta-background-color);
    border: 1px solid var(--secondary-button-cta-border-color);
    color: var(--hvid);
    padding: 0.5rem 30px;
    display: inline-block;
    box-shadow: inset 0 0 0 0 var(--orange-800);
    -webkit-transition: ease-out 0.4s;
    -moz-transition: ease-out 0.4s;
    transition: ease-out 0.4s;
    white-space: nowrap;
    margin-left: 2rem;
  }

  button:hover {
    border: 1px solid var(--orange-light);
    box-shadow: inset 400px 0 0 0 #ff853e;
    color: var(--hvid);
  }

  .mobile-icon {
    width: 25px;
    height: 14px;
    position: relative;
    cursor: pointer;
  }

  .mobile-icon:after,
  .mobile-icon:before,
  .middle-line {
    content: "";
    position: absolute;
    width: 100%;
    height: 2px;
    background-color: #fff;
    transition: all 0.4s;
    transform-origin: center;
  }

  .mobile-icon:before,
  .middle-line {
    top: 0;
  }

  .mobile-icon:after,
  .middle-line {
    bottom: 0;
  }

  .mobile-icon:before {
    width: 66%;
  }

  .mobile-icon:after {
    width: 33%;
  }

  .middle-line {
    margin: auto;
  }

  .mobile-icon:hover:before,
  .mobile-icon:hover:after,
  .mobile-icon.active:before,
  .mobile-icon.active:after,
  .mobile-icon.active .middle-line {
    width: 100%;
  }

  .mobile-icon.active:before,
  .mobile-icon.active:after {
    top: 50%;
    transform: rotate(-45deg);
  }

  .mobile-icon.active .middle-line {
    transform: rotate(45deg);
  }

  .navbar-list {
    display: none;
    width: 100%;
    justify-content: space-between;
    margin: 0;
  }

  .navbar-list.mobile {
    background-color: rgba(0, 0, 0, 0.8);
    position: fixed;
    display: block;
    height: calc(100% - 100px);
    bottom: 0;
    left: 0;
    /* width: 100vw; */
  }

  .navbar-list li {
    list-style-type: none;
    position: relative;
  }

  .navbar-list li:before {
    content: "";
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 1px;
    background-color: black;
  }

  .navbar-list a {
    color: #fff;
    text-decoration: none;
    display: flex;
    height: 45px;
    align-items: center;
    padding: 0 10px;
    font-size: 13px;
  }

  label:after {
    content: "+";
    position: absolute;
    right: 1em;
    color: #fff;
  }

  input:checked + label:after {
    content: "-";
    line-height: 0.8em;
  }

  .accordion__content {
    max-height: 0em;
    transition: all 0.4s cubic-bezier(0.865, 0.14, 0.095, 0.87);
  }
  input[name="panel"]:checked ~ .accordion__content {
    /* Get this as close to what height you expect */
    max-height: 50em;
  }

  #hover_underkategori {
    width: 56rem;
  }

  #topnav_titel {
    font-size: var(--font_h4);
  }

  @media only screen and (min-width: 1000px) {
    .mobile-icon {
      display: none;
    }

    .navbar-list {
      display: flex;
      padding: 0;
    }

    .navbar-list a {
      display: inline-flex;
    }
  }

  @media only screen and (max-width: 1000px) {
    button {
      display: none;
    }
  }
</style>
