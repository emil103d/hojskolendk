<script>
  export let type = "default";
</script>

<button class={type}> <slot /> </button>

<style>
  /* -----MODE=PRIMARY START --------- */

  button,
  .primary {
    font-size: var(--knapsize);
    font-weight: bold;
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
    box-shadow: inset 400px 0 0 0
      var(--primary-button-cta-background-color-hover);
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

  /* -----MODE=LINK START --------- */
  .linkbutton {
    color: var(--txtcolor-600);
    background-color: transparent;
    box-shadow: none;
    border-bottom: 1px solid rgb(163, 162, 162);
    border-radius: 0;
    padding: 0;
    display: grid;
    grid-template-columns: 1fr auto;
    gap: 1rem;
    border: 1px solid white;
  }

  .linkbutton:hover {
    background-color: transparent;
    border: 1px solid white;
    border-bottom: 1px solid var(--txtcolor-600);
    box-shadow: none;
    color: var(--txtcolor);
    -webkit-transition: ease-out 0s;
    -moz-transition: ease-out 0s;
    transition: ease-out 0s;
  }

  /* -----MODE=GHOST START --------- */
  .ghostbutton {
    color: white;
    background-color: var(--button-ghost-background-color);
  }

  .ghostbutton:hover {
    background-color: var(--button-ghost-background-color);
    color: grey;
    cursor: default;
  }

  /* <!-- <svg
    width="18"
    height="8"
    viewBox="0 0 18 8"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M17.3536 4.35355C17.5488 4.15829 17.5488 3.84171 17.3536 3.64645L14.1716 0.464466C13.9763 0.269204 13.6597 0.269204 13.4645 0.464466C13.2692 0.659728 13.2692 0.976311 13.4645 1.17157L16.2929 4L13.4645 6.82843C13.2692 7.02369 13.2692 7.34027 13.4645 7.53553C13.6597 7.7308 13.9763 7.7308 14.1716 7.53553L17.3536 4.35355ZM17 3.5L0 3.5V4.5L17 4.5V3.5Z"
      fill="#929292"
    />
  </svg> --> */
</style>
