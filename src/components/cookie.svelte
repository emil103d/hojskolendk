<script>
  let isOpen = true;

  export function closeModal() {
    isOpen = false;
    reset();
  }
</script>

{#if isOpen}
  <div class="cookie w-96 fixed z-5000 pb-5 bg-white">
    <div>
      <img class="" src="../src/_icons/cookie.png" alt="" />
      <div class="px-4 m-4">
        <h3>Vi anvender cookie</h3>
        <p>
          Denne hjemmeside bruger cookies for at fungere, til brug for
          trafikmåling og optimering af sidens indhold samt til at målrette
          markedsføring. Ved at bruge vores side accepterer du brug af cookies
          til disse formål.
        </p>
        <div class="m-auto">
          <div class="flex gap-2 my-6 ml-8">
            <button on:click={closeModal} class="primary">Accepter</button>
            <button class="secondary"
              ><a href="/underconstruction">Læs mere</a></button
            >
          </div>
        </div>
      </div>
    </div>
  </div>
{/if}

<style>
  .cookie {
    z-index: 100;
    bottom: 10%;
    right: 3%;
  }

  .primary {
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
  }

  button:hover,
  .primary:hover {
    border: 1px solid var(--orange-light);
    box-shadow: inset 400px 0 0 0 #ff853e;
    color: var(--hvid);
  }

  /* -----MODE=SECONDARY START --------- */

  .secondary {
    font-family: "lato";
    background-color: var(--hvid);
    color: var(--textcolor);
    border: 1px solid var(--secondary-button-cta-border-color);
    padding: 0.5rem 30px;
    display: inline-block;
    box-shadow: inset 0 0 0 0 #ff5e04;
    -webkit-transition: ease-out 0.4s;
    -moz-transition: ease-out 0.4s;
    transition: ease-out 0.4s;
  }

  .secondary:hover {
    background-color: var(--button-cta-background-color-hover);
    color: var(--hvid);
    border: solid 1px white;
  }
</style>
