<script>
  export let title;
  export let image;
  export let addon;
  export let text;
</script>

<div class="shadox mx-auto my-8 relative z-0 overflow-hidden object-cover">
  <img class="hover:scale-105 object-cover" src={image} alt={title} />
  <div class="bg-white pl-3 pr-3 pt-3 pb-3 z-3 absolute top-4 max-h-full">
    <h3 class="text-sm">
      {title}
    </h3>
    <p class="lilletekst">{addon}</p>
  </div>
  <p class="mt-3 m-3">{text}</p>
</div>

<style>
  img {
    height: 24rem;
    width: auto;
    transition: all 0.2s ease-in-out;
  }

  .shadox {
    box-shadow: 7px 5px 14px rgba(0, 0, 0, 0.07);
    min-height: 24rem;
    min-width: 15rem;
    transition: transform 0.2s;
  }

  .lilletekst {
    color: var(--orange);
    font-size: var(--font_preh2);
    padding: var(--spacing-10);
    line-height: var(--line-s);
  }
</style>
