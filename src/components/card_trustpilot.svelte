<script>
  export let text;
  export let name;
  export let image;
  export let title;
</script>

<div class="bg-slate-400 max-w-xs relative rounded h-96">
  <img
    class="absolute -top-10 left-1/2 rounded-full w-20 h-20"
    src={image}
    alt=""
  />
  <div class="m-4 mt-14">
    <img
      class="w-24 h-auto justify-center mx-auto"
      src="../src/_icons/5star.png"
      alt=""
    />
    <h3>{title}</h3>
    <p>
      {text}
    </p>
    <p>- {name}</p>
  </div>
</div>
