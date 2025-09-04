<script>
  import Scroller from "../lib/Scroller.svelte";
  import ArticleText from "../lib/ArticleText.svelte";
</script>

<div class="image-container">
  <Scroller layout="right">
    {#snippet sticky()}
      <img
        class="main-image"
        src="/kwk-scrollytelling-template/fourthpage_photo.jpg"
        alt="BWDC screenshot"
      />
      <div class="image-caption">
        <p>
          This is a screenshot from the <a
            href="https://blackwealthdata.org/explore/business">BWDC website</a
          >
        </p>
      </div>
    {/snippet}

    {#snippet scrolly()}
      <ArticleText>
        After discussing PPP loans, lets shift over to this chart, which
        displays the growth and equity in entrepreneurship for Cumberland County
      </ArticleText>

      <ArticleText>
        The economic opportunities/challenges (i.e. PPP loan distribution) could
        be a factor to why business formations are a little less in this county
        compared to the national.
      </ArticleText>

      <ArticleText>
        If Black-owned businesses face greater barriers to startup capital, they
        may struggle with revenue, profitability, and sustaining employment.
        This suggests that the unequal access to capital is an important factor
        behind the differences in business outcomes.
      </ArticleText>
    {/snippet}
  </Scroller>
</div>

<style>
  .main-image {
    width: 500px;
    height: 350px;
    border-radius: 10px;
    box-shadow: 0 4px 12px;
  }
</style>
