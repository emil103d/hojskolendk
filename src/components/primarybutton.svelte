<script></script>

<button class="primarybutton"> <slot /> </button>

<style>
  button,
  .primarybutton {
    background-color: var(--orange);
    font-size: var(--font_knap_m);
    line-height: var(--line-l);
    padding: var(--spacing-button);
    font-size: var(--font_knap_m);
    font-weight: 400;
    color: var(--hvid);
    border: 1px solid var(----primary-button-cta-background-color);
  }

  button:hover,
  .primarybutton:hover {
    border: var(--button-cta-background-color-hover);
    background-color: var(--button-cta-background-color-hover);
  }
</style>
