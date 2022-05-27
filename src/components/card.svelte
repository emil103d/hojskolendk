<script>
  export let title;
  export let image;
</script>

<div class="rounded overflow-hidden shadow-lg mx-auto my-8 relative z-0">
  <img
    class=" object-cover w-full z-1 transition hover:scale-125"
    src={image}
    alt="billede af vand"
  />
  <h3 class="bg-white pl-3 pt-3 pb-3 pr-0 z-3 absolute top-4 text-xs">
    {title}
  </h3>
</div>

<style>
  div {
    min-height: 24rem;
  }

  img {
    height: 24rem;
    width: 14rem;
  }
</style>
