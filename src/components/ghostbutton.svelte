<script></script>

<button class="ghostbutton">
  <slot />
</button>

<style>
  .ghostbutton {
    color: white;
    background-color: var(--button-ghost-background-color);
  }

  .ghostbutton:hover {
    background-color: var(--button-ghost-background-color);
    color: grey;
    cursor: default;
  }
</style>
