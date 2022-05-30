<script>
  export let title;
  export let image;
</script>

<div class=" mx-auto my-8 relative z-0">
  <img class="hover:scale-105" src={image} alt={title} />
  <h3 class="bg-white pl-3 pt-3 pb-3 pr-3 z-3 absolute top-4 text-xs">
    {title}
  </h3>
</div>

<style>
  div {
    min-height: 24rem;
    min-width: 15rem;
    transition: transform 0.2s;
  }

  img {
    height: 24rem;
    width: 15rem;
  }

  /* div:hover {
    transform: scale(1.1);
  } */
</style>
