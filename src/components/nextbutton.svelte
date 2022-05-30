<script></script>

<button class="nextbutton">
  <slot />
  <svg
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
  </svg>
</button>

<style>
  .nextbutton {
    color: var(--txtcolor-600);
    background-color: transparent;
    box-shadow: none;
    border-bottom: 1px solid rgb(163, 162, 162);
    border-radius: 0;
    padding: 0;
    display: flex;
    flex-direction: row;
  }
  .nextbutton svg {
    margin: auto 0px auto 10px;
  }
  .nextbutton:hover {
    font-weight: 500;
    background-color: transparent;
    border-bottom: 1px solid var(--txtcolor-600);
  }
</style>
