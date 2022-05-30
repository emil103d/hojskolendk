<script></script>

<button class="secondarybutton"> <slot /> </button>

<style>
  .secondarybutton {
    white-space: nowrap;
    background-color: var(--secondary-button-cta-background-color);
    border: solid 1px white;
    padding: var(--spacing-button);
    color: var(--txtcolor);
    font-weight: 500;
  }

  .secondarybutton:hover {
    background-color: var(--button-cta-background-color-hover);
    color: var(--hvid);
    border: solid 1px white;
  }
</style>
