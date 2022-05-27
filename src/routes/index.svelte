<script>
</script>

<svelte:head><title>Forside</title></svelte:head>

<section />

<style>
  .ru-parallax-reveal-outer-container {
    max-width: 600px;
    margin: auto;
    width: 90%;
    padding: 200px 0px;
    position: relative;
  }

  .ru-parallax-reveal-outer-container > .image-container {
    padding-bottom: 100%;
    background: black;
    position: relative;
    overflow: hidden;
    z-index: 2;
    background-size: cover;
    background-position: center;
  }

  .ru-section-title {
    margin: 0;
    font-size: 64px;
    width: 100%;
    text-align: center;
    position: absolute;
    top: 50%;
    left: -30%;
    transform: translateY(-50%);
    z-index: 1;
    white-space: nowrap;
  }
  .ru-section-title.on-dark {
    color: white;
  }
  .ru-section-title span {
    position: relative;
    display: block;
  }
</style>
