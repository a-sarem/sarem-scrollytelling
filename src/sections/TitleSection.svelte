<script>
  import TitleCard from "../lib/TitleCard.svelte";

  const title =
    "Disparities in Profitability: A Study of Race & Business Ownership";
  const subtitle = "By Sarem Agha";
</script>

<div class="background-container">
  <TitleCard {title} {subtitle} />
</div>

<style>
  .background-container {
    background-image: url("./titlepage_background.jpg");
    background-size: cover;
    height: auto;
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat;
  }
</style>
