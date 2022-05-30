<script>
  export let imgtitle;
  import MyButton from "./primarybutton.svelte";
</script>

<section>
  <img src={imgtitle} alt="herobillede" class="hero-image" />
  <div class="hero-text">
    <h2>UNDSKYLD VI RODER</h2>
    <p>Siden er ved at blive bygget men</p>
    <p>tag en rundrejse på vores andre sider imens</p>
    <MyButton><a href="__layout.svelte">TAG MIG TILBAGE</a></MyButton>
  </div>
</section>

<style>
  section {
    margin-left: auto;
    margin-right: auto;
  }

  .hero-text {
    background-color: rgba(255, 255, 255, 0.672);
    padding: 1rem;
    border-radius: var(--border-radius-sm);
  }

  p {
    color: black;
  }
</style>
