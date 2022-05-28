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
    const mediaListener = window.matchMedia("(max-width: 767px)");

    mediaListener.addListener(mediaQueryHandler);
  });
</script>

<nav class="w-screen grid grid-cols-10 md:grid-cols-3">
  <img class="cols-span-4" src="../src/_logo/logohvid.png" alt="logo hvid" />
  <div class="inner cols-span-6 justify-center ">
    <div
      on:click={handleMobileIconClick}
      class={`mobile-icon${showMobileMenu ? " active" : ""}`}
    >
      <div class="middle-line" />
    </div>
    <ul class={`navbar-list${showMobileMenu ? " mobile" : ""}`}>
      <li id="" class="bg-black">
        <div
          class="accordion justify-center flex-col flex overflow-y-scroll pb-10 flex-nowrap"
        >
          <!--  Panel 1  -->
          <div class="">
            <input type="checkbox" name="panel" id="panel-1" class="hidden" />
            <p
              for="panel-1"
              class="relative block bg-black text-white p-4 shadow border-b border-grey"
            >
              Se alle ophold
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
                <li class="text-white"><a href="/singlepage">xxxx</a></li>
                <li class="text-white"><a href="/singlepage">xxxx</a></li>
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
                  <a href="/singlepage">AUSTRALIEN, NZ, BALI & GILI ISLANDS</a>
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
              Infomøder
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
                  <a href="/#">Mød teamet</a>
                </li>
                <li class="text-white">
                  <a href="/#">Vores Værdier</a>
                </li>
                <li class="text-white">
                  <a href="/#">Bæredygtighed</a>
                </li>
                <li class="text-white">
                  <a href="/#">FAQ</a>
                </li>
                <li class="text-white">
                  <a href="/#">Blog</a>
                </li>

                <li class="text-white">
                  <a href="/#">Det siger vores elever</a>
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
            <div class="accordion__content overflow-hidden bg-grey-lighter">
              <ul class="accordion__body p-4" id="panel1">
                <li class="text-white"><a href="/#">Kommende Events</a></li>
                <li class="text-white"><a href="/#">Elev Ambasadører</a></li>
                <li class="text-white"><a href="/#">REUNION</a></li>
              </ul>
            </div>
          </div>
        </div>
      </li>

      <li class="hidden md:block">
        <div class="group relative h-full">
          <a
            href="#"
            class="text-white flex items-center h-full bg-grey-darkest px-4"
          >
            Account
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
            <a
              href="#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              My Account
            </a>
            <a
              href="#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              Edit Account
            </a>
            <a
              href="#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              Logout
            </a>
          </div>
        </div>
      </li>
      <li class="hidden md:block">
        <div class="group relative h-full">
          <a
            href="#"
            class="text-white flex items-center h-full bg-grey-darkest px-4"
          >
            Account
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
            <a
              href="#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              My Account
            </a>
            <a
              href="#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              Edit Account
            </a>
            <a
              href="#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              Logout
            </a>
          </div>
        </div>
      </li>
      <li class="hidden md:block">
        <div class="group relative h-full">
          <a
            href="#"
            class="text-white flex items-center h-full bg-grey-darkest px-4"
          >
            Account
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
            <a
              href="#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              My Account
            </a>
            <a
              href="#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              Edit Account
            </a>
            <a
              href="#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              Logout
            </a>
          </div>
        </div>
      </li>
      <li class="hidden md:block">
        <div class="group relative h-full">
          <a
            href="/#"
            class="text-white flex items-center h-full bg-grey-darkest px-4"
          >
            Account
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
            <a
              href="/#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              My Account
            </a>
            <a
              href="/#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              Edit Account
            </a>
            <a
              href="/#"
              class="block text-left py-3 px-3 text-white hover:text-blue-dark text-xs"
            >
              Logout
            </a>
          </div>
        </div>
      </li>
    </ul>
    <button class="hidden md:block">TILMELD INFOMØDE</button>
  </div>
</nav>

<!------------------- Credits   ---------------------->

<!-- https://linguinecode.com/post/create-a-navbar-in-svelte -->
<style>
  nav {
    background: #000000;
    opacity: 0.7;
    backdrop-filter: blur(58px);
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
  .inner {
    max-width: 980px;
    padding-left: 20px;
    padding-right: 10%;
    margin: auto;
    box-sizing: border-box;
    display: flex;
    align-items: center;
    height: 100%;
    width: 40rem;
  }

  button {
    margin-left: 2rem;
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
    padding: 0 40px;
  }

  .navbar-list.mobile {
    background-color: rgba(0, 0, 0, 0.8);
    position: fixed;
    display: block;
    height: calc(100% - 100px);
    bottom: 0;
    left: 0;
    width: 100vw;
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

  @media only screen and (min-width: 767px) {
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
</style>
