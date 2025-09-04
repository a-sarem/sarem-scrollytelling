<script>
  import TitleCard from "../lib/TitleCard.svelte";

  const title = "Thank you!";
  const subtitle = "Sarem Agha";
</script>

<div class="background-container">
  <TitleCard {title} {subtitle} />
</div>

<style>
  .background-container {
    background-image: url("/titlepage_background.jpg");
    background-size: cover;
    height: auto;
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat;
  }
</style>
