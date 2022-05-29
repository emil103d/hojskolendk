<script>
  import Card from "../components/card.svelte";
  import { fade, scale } from "svelte/transition";
  import { flip } from "svelte/animate";

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

  const rotateleft = (e) => {
    array = [array[array.length - 1], ...array.slice(0, array.length - 1)];
  };

  const rotateright = (e) => {
    array = [...array.slice(1, array.length), array[0]];
  };
</script>

<div id="carosoule_container">
  <div class="flex gap-5 justify-center items-center flex-nowrap w-96">
    {#each array as item (item.id)}
      <div
        id={item.id}
        animate:flip={{ duration: 300 }}
        out:scale={{ duration: 250 }}
        in:scale={{ duration: 250 }}
      >
        <Card image="../src/_images/1.jpg" title={"Hej med dig"} />
      </div>
    {/each}
  </div>

  <button on:click={rotateleft}><img src="../src/" alt="" /></button>
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
