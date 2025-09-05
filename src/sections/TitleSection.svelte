<script>
  import TitleCard from "../lib/TitleCard.svelte";
  import titleBg from "/titlepage_background.jpg";

  const title =
    "Disparities in Profitability: A Study of Race & Business Ownership";
  const subtitle = "By Sarem Agha";
</script>

<div class="background-container" style="background-image: url({titleBg})">
  <TitleCard {title} {subtitle} />
</div>

<style>
  .background-container {
    background-size: cover;
    height: auto;
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat;
  }
</style>
