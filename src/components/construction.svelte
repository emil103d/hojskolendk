<script>
  import MyButton from "../components/button.svelte";
</script>

<section class="maxwidthwrapper">
  <img src="buda.png" alt="herobillede" class="fly mt-20" />
  <div class="hero-text">
    <h2>UNDSKYLD VI RODER</h2>
    <p>Siden er ved at blive bygget men</p>
    <p>tag en rundrejse på vores andre sider imens</p>
    <div class="m-10">
      <MyButton type="primary">
        <a href="index.svelte"> TILBAGE TIL FORSIDEN </a></MyButton
      >
    </div>
  </div>
</section>

<style>
  section {
    margin-left: auto;
    margin-right: auto;
    min-height: 600px;
  }
  p,
  h2 {
    color: var(--txtcolor);
  }

  img {
    width: 1000px;
  }

  .fly {
    animation-name: fly;
    animation-duration: 2s;
    animation-fill-mode: both;
  }

  @keyframes fly {
    0% {
      transform: rotateX(50deg) translateX(-50vw) skewX(-50deg);
      opacity: 1;
    }
    100% {
      transform: rotateX(0deg) translateX(0) skewX(0deg);
      opacity: 1;
    }
  }
</style>
