<script>
  export let title;
  export let image;
  export let addon;
  export let text;
</script>

<div class="shadox mx-auto my-8 relative z-0 overflow-hidden ">
  <img class="hover:scale-105" src={image} alt={title} />
  <div class="bg-white pl-3 pt-3 pb-3 z-3 absolute top-4 max-h-full">
    <h3 class=" text-sm">
      {title}
    </h3>
    <p class="lilletekst">{addon}</p>
  </div>
  <p>{text}</p>
</div>

<style>
  img {
    height: 24rem;
    width: 15rem;
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
