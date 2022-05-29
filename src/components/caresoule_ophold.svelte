<script>
  import Card from "../components/card.svelte";
  import { fade, scale } from "svelte/transition";
  import { flip } from "svelte/animate";
  export let speed = 1000;

  let array = [
    {
      id: 0,
    },
    {
      id: 1,
    },
    {
      id: 2,
    },
    {
      id: 3,
    },
    {
      id: 4,
    },
    {
      id: 5,
    },
    {
      id: 6,
    },
  ];
  let returned = "";

  const rotateleft = (e) => {
    const transitioningArray = array[array.length - 1];
    document.getElementById(transitioningArray.id).style.opacity = 0;
    array = [array[array.length - 1], ...array.slice(0, array.length - 1)];
    setTimeout(
      () => document.getElementById(transitioningArray.id).style.opacity - 1,
      speed
    );
  };

  const rotateright = (e) => {
    const transitioningArray = array[array.length - 1];
    document.getElementById(transitioningArray.id).style.opacity = 0;
    array = [...array.slice(1, array.length), array[0]];
    setTimeout(
      () => document.getElementById(transitioningArray.id).style.opacity - 1,
      speed
    );
  };
</script>

<div id="carosoule_container">
  <h3>array:</h3>
  <div class="flex gap-5 justify-center items-center flex-nowrap ">
    {#each array as item (item.id)}
      <div
        animate:flip={{ duration: speed }}
        out:scale={{ duration: 250 }}
        in:scale={{ duration: 250 }}
      >
        <Card image="../src/_images/1.jpg" title={item.id} />
      </div>
    {/each}
  </div>

  <button on:click={rotateleft}>Left</button>
  <button on:click={rotateright}>Right</button>
</div>

<style>
  #carosoule_container {
    width: 100%;
    overflow-x: hidden;
    margin-left: 5rem;
    margin-right: 5rem;
  }
</style>
