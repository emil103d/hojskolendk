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

<nav class="grid grid-cols-2 md:grid-cols-3">
  <img class="cols-1" src="../src/_logo/logohvid.png" alt="logo hvid" />
  <div class="inner cols-2">
    <div
      on:click={handleMobileIconClick}
      class={`mobile-icon${showMobileMenu ? " active" : ""}`}
    >
      <div class="middle-line" />
    </div>
    <ul class={`navbar-list${showMobileMenu ? " mobile" : ""}`}>
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
    width: 100%;
  }

  img {
    width: 4rem;
    margin: 1rem;
    grid-column: 2;
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
    grid-column: 3;
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
    height: calc(100% - 45px);
    bottom: 0;
    left: 0;
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
