<script>
  import ContentOverlay from "./ContentOverlay.svelte";
  import Footer from "./Footer.svelte";
  import "./global.css";
</script>

<svelte:head>
  <title>Sticky Footer</title>
</svelte:head>

<ContentOverlay />
<div class="overlay">
  <div class="overlay__fixed">
    <Footer />
  </div>
</div>

<style>
  .overlay {
    position: relative;
    height: 600px;
  }

  .overlay__fixed {
    position: fixed;
    width: 100%;
    bottom: 0;
  }
</style>
