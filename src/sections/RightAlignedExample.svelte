<script>
  import Scroller from "../lib/Scroller.svelte";
  import ArticleText from "../lib/ArticleText.svelte";
</script>

<div class="scrolly-section">
  <Scroller layout="right">
    {#snippet sticky()}
      <div class="image-container">
        <img
          src="/kwk-scrollytelling-template/secondpage_photo.jpg"
          alt="Business owner picture"
          class="main-image"
        />
      </div>
    {/snippet}

    {#snippet scrolly()}
      <ArticleText>
        Wealth inequality in the U.S. are tied down to our historical roots and
        racial wealth gaps is a huge challenge for us to this day.
      </ArticleText>

      <ArticleText>
        We will focusing on Black-owned businesses and their access to loans and
        financial support shown in the <a href="https://blackwealthdata.org/"
          >Black Wealth Data Center.</a
        >
      </ArticleText>

      <ArticleText>
        The data shown will be focused in <strong
          >Cumberland County, North Carolina.
        </strong>
      </ArticleText>

      <ArticleText>
        This project will try to answer this question: <br /><br />

        <strong
          >“What are the key differences in business outcomes (revenue,
          profitability, employment, etc.) between Black-owned and white-owned
          businesses, and how much of that can be attributed to disparities in
          access to capital?”</strong
        >
      </ArticleText>
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
</style>
