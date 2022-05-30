<script>
  export let title;
  export let image;
</script>

<div class="rounded overflow-hidden shadow-lg mx-auto my-8 relative z-0">
  <img src={image} alt={title} />
  <h3 class="bg-white pl-3 pt-3 pb-3 pr-0 z-3 absolute top-4 text-xs">
    {title}
  </h3>
</div>

<style>
  div {
    min-height: 24rem;
    min-width: 15rem;
  }

  img {
    height: 24rem;
    width: 15rem;
  }
</style>
