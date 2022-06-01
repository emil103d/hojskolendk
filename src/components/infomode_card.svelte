<script>
  export let image;
  export let title;
  export let subtitle;
  export let dato;
  export let tid;
  export let adresse;
  import MyButton from "../components/button.svelte";
</script>

<section
  class="ophold max-w-full h-full block md:flex items-center mb-5 grid">
  <div class="">
    <img src={image} alt={title} class="w-full object-cover md:w-40 mr-10" />
  </div>

  <div class="pb-4">
    <div class="m-5">
      <h3>{title}</h3>
      <p>{subtitle}</p>
    </div>
    <div class="md:flex mt-10 m-5 ">
      <div class="flex mt-3">
        <img class="w-8 h-8 mr-6" src="../src/_icons/calender.png" alt="" />
        <div class="">
          <p class="">Dato:</p>
          <p class="tabeltxt">{dato}</p>
        </div>
        <div class="h-10 hidden md:block bg-black w-0.5 ml-3 mr-6" />
      </div>
      <div class="flex mt-5">
        <img class="w-8 h-8 mr-5" src="../src/_icons/calender.png" alt="" />
        <div>
          <p class="">Tid:</p>
          <p class="tabeltxt">{tid}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6 hidden md:block" />
      </div>
      <div class="flex mt-5 ">
        <img class="w-8 h-8 mr-5" src="../src/_icons/price.png" alt="" />
        <div class="w-22">
          <p class="">Adresse:</p>
          <p class="tabeltxt ">{adresse}</p>
        </div>
        <div class="h-10 bg-black w-0.5 ml-3 mr-6 hidden md:block" />
      </div>
    </div>
  </div>

  <div class="flex justify-center">
    <MyButton type="primary">Tilmeld infomøde</MyButton>
  </div>
</section>

<style>
  .ophold {
    margin: 5px;
    background-color: var(--sandbeach);
    margin-bottom: 2rem;
  }

  .right svg {
    height: 25px;
    width: 25px;
  }

  .right {
    background-color: white;
    border-radius: 50px;
    height: 60px;
    width: 60px;
    z-index: 10;
  }

  @media screen and (max-width: 400px) {
    section {
      max-width: 100px;
    }
  }
</style>
