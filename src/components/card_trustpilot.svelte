<script>
  export let text;
  export let name;
  export let image;
  export let title;
</script>

<div class="trustcard max-w-xs rounded relative p-2">
  <img
    class="rounded-full w-28 h-28 -mt-24 border-white border-4 justify-center absolute -top-14 left-24"
    src={image}
    alt="avatar billede af anmelderen"
  />
  <div class="m-4 mt-14">
    <img
      class="w-24 h-auto justify-center mx-auto py-4"
      src="5star.png"
      alt="trustpulot 5 stjerner"
    />
    <h3>{title}</h3>
    <p>
      {text}
    </p>
    <p><br /> - {name}</p>
  </div>
</div>

<style>
  .trustcard {
    background-color: var(--sandbeach);
  }

  p {
    color: var(--txtcolor-700);
  }

  img {
    margin: 0 auto;
  }
</style>
