<script>
  import { opholdData } from "../stores/opholdData.js";
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

<div class="">
  <section class="maxwidthwrapper">
    <div id="carowrapper">
      <button id="left" on:click={rotateleft}
        ><svg
          width="42"
          height="66"
          viewBox="0 0 42 66"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M39.4561 62.7832L4.78214 31.6962L39.4561 3.0006"
            stroke="black"
            stroke-width="6"
          />
        </svg>
      </button>
      <div id="carosoule_container">
        <div class="flex gap-5 items-center flex-nowrap z-2 w-96">
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
      </div>
      <button id="right" on:click={rotateright}
        ><svg
          width="43"
          height="66"
          viewBox="0 0 43 66"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M2.95605 2.92773L37.8401 34.2031L2.95605 63.0727"
            stroke="black"
            stroke-width="6"
          />
        </svg>
      </button>
    </div>
  </section>
</div>

<style>
  #carosoule_container {
    /* width: 700px; */
    overflow-x: hidden;
    margin-left: 10rem;
    margin-right: 10rem;
    z-index: 1;
    padding-left: 50px;
    padding-right: 50px;
  }

  #carowrapper {
    position: relative;
  }

  #left svg {
    height: 25px;
    width: 25px;
  }

  #right svg {
    height: 25px;
    width: 25px;
  }

  #left {
    background-color: white;
    border-radius: 50px;
    height: 60px;
    width: 60px;
    top: 40%;
    left: 13%;
    position: absolute;
    z-index: 10;
  }

  #right {
    background-color: white;
    border-radius: 50px;
    height: 60px;
    width: 60px;
    top: 40%;
    right: 8%;
    position: absolute;
    z-index: 10;
  }
  #left:hover,
  #right:hover {
    height: 62px;
    width: 62px;
  }

  /* #left {
    position: absolute;
    top: 0%;
    left: 20%;
    z-index: 10;
  }

  #right {
    position: absolute;
    top: 50%;
    right: 50%;
  } */
</style>
