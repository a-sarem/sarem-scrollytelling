<script>
  import { blur, slide } from "svelte/transition";
  import Scroller from "../lib/Scroller.svelte";
  import ObservedArticleText from "../lib/ObservedArticleText.svelte";
  import ArticleText from "../lib/ArticleText.svelte";
  import ImageExample from "./ImageExample.svelte";
</script>

<div class="image-container">
  <Scroller layout="left">
    {#snippet sticky()}
      <img
        class="main-image"
        src="/kwk-scrollytelling-template/fifthpage_photo.jpg"
        alt="BWDC screenshot"
      />
    {/snippet}

    {#snippet scrolly()}
      <ArticleText>
        Looking statewide, North Carolina has over 9,000 Black-owned employer
        firms, with a Black population of 20.6%. Which shows strong
        representation in entrepreneurship.
      </ArticleText>

      <ArticleText>
        Even in a state with high Black business ownership, unequal outcomes
        still exist, which suggests that access to capital (not just the number
        of firms) is a major factor
      </ArticleText>

      <ArticleText>
        But if we go back to my original question, do these businesses achieve
        the same outcomes as white-owned firms? How much of that gap is
        explained by unequal access to capital, such as disparities in loan
        approvals or investment opportunities?
      </ArticleText>
    {/snippet}
  </Scroller>
</div>

<style>
  .main-image {
    width: 500px;
    height: 350px;
    object-fit: fit;
    border-radius: 10px;
    box-shadow: 0 4px 12px;
  }

  .list {
    margin: 0px 20px;
    background-color: #ff99fc;
    color: #8427c9;
    border: solid #8427c9 3px;
    border-radius: 20px;
    box-shadow: 16px 16px #8aa6df;
    width: 100%;
  }

  h3 {
    text-align: center;
  }
</style>
