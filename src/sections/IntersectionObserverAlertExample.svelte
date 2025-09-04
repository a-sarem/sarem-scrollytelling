<script>
  import { blur, slide } from "svelte/transition";
  import Scroller from "../lib/Scroller.svelte";
  import ObservedArticleText from "../lib/ObservedArticleText.svelte";
  import ArticleText from "../lib/ArticleText.svelte";
  import ImageExample from "./ImageExample.svelte";
</script>

<div class="image-container">
  <Scroller layout="right">
    {#snippet sticky()}
      <img
        class="main-image"
        src="/kwk-scrollytelling-template/finalpage_photo.jpg"
        alt="BWDC screenshot"
      />
    {/snippet}

    {#snippet scrolly()}
      <ArticleText
        >In Cumberland County, fewer businesses are being formed compared to the
        national level, while statewide North Carolina has a strong presence of
        Black-owned employer firms.</ArticleText
      >

      <ArticleText
        >Research consistently shows that Black-owned businesses, on average,
        generate lower revenue, employ fewer workers, and have lower
        profitability than white-owned firms.</ArticleText
      >
      <ArticleText>
        From <a
          href="https://www.jpmorganchase.com/institute/news-events/small-business-in-black-and-hispanic-communities"
          >JP Morgan Chase</a
        >, their article states: “In over 88 percent of majority black or
        Hispanic communities, the median profit margin is 15 percent or less.
        Only 35 percent of majority White communities have median profit margins
        below this threshold.”
      </ArticleText>

      <ArticleText
        >Understanding how unequal access to capital impacts differences in
        revenue, profitability, and employment, and it is important to bring
        this up when addressing the unequal outcomes between Black-owned and
        White-owned businesses.</ArticleText
      >
    {/snippet}
  </Scroller>
</div>

<style>
  .main-image {
    width: 700px;
    height: 450px;
    object-fit: cover;
    border-radius: 10px;
    box-shadow: 0 4px 12px;
  }

  h3 {
    text-align: center;
  }
</style>
