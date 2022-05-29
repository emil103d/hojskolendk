<script>
  export let imgtitle;
</script>

<img src={imgtitle} alt="herobillede" class="hero-image" />
<div class="hero-text">
  <p>Rejs med HÔJSKOLENDK til</p>
  <h2>SRI LANKE, MALDIVERNE & THAILAND</h2>
</div>

<style>
  .hero-image {
    height: 80%;
    width: 100%;
    top: 0%;
    left: 0%;
  }
  .hero-text {
    text-align: center;
    position: absolute;
    top: 50%;
    left: 55%;
    transform: translate(-50%, -50%);
    color: white;
  }

  .hero-text h2 {
    color: var(--hvid);
  }
</style>
