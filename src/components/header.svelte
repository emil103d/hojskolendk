<script>
  export let imgtitle;
  export let subtitle;
  export let title;
</script>

<img src={imgtitle} alt="herobillede" class="hero-image" />
<div class="hero-text">
  <p>{subtitle}</p>
  <h2>{title}</h2>
</div>

<style>
  .hero-text h2 {
    color: var(--hvid);
  }
</style>
