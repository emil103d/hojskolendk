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
      <div class="px-4">
        <h3>Vi anvender cookie</h3>
        <p>
          Denne hjemmeside bruger cookies for at fungere, til brug for
          trafikmåling og optimering af sidens indhold samt til at målrette
          markedsføring. Ved at bruge vores side accepterer du brug af cookies
          til disse formål.
        </p>
        <div class="flex">
          <button on:click={closeModal}>Accepter</button>
          <button><a href="/underconstruction">Læs mere</a></button>
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
</style>
