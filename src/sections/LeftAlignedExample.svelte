<script>
  import * as Highcharts from "highcharts";
  import "highcharts/modules/exporting";
  import { Chart } from "@highcharts/svelte";
  import Scroller from "../lib/Scroller.svelte";
  import ArticleText from "../lib/ArticleText.svelte";
</script>

<div>
  <Scroller layout="left">
    {#snippet sticky()}
      <div class="image-container">
        <img
          src="/kwk-scrollytelling-template/thirdpage_photo.jpg"
          alt="Screenshot of BWDC website showing business support data"
          class="main-image"
        />

        <div class="image-caption">
          <p>
            This is a screenshot from the <a
              href="https://blackwealthdata.org/wealth-indicator?firstCounty=Cumberland%20County,%20North%20Carolina&secondCounty=national&method=auto"
              >BWDC website</a
            >
          </p>
        </div>
      </div>
    {/snippet}

    {#snippet scrolly()}
      <ArticleText>
        The data can display the inequities in business support, particularly
        for Black-owned businesses in Cumberland County, compared to the
        national average.
      </ArticleText>

      <ArticleText>
        It also shows how access to capital was not equal. During COVID-19, PPP
        Loans (a federal funding program to support small businesses through
        COVID-19) was not distributed equally.
      </ArticleText>

      <ArticleText>
        Additionally, this reflects access to emergency small business loans and
        highlights the disparities in how financial relief distributed.
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

  .toggle-button {
    margin: 20px;
    padding: 20px;
    color: #007052;
    background-color: #0bd956;
    border: solid 2px #007052;
    border-radius: 16px;
    font-size: large;
    cursor: pointer;
    transition: all 0.2s ease;
    box-shadow: 0 4px 0 #007052;
  }

  .toggle-button:active {
    transform: translateY(2px);
    box-shadow: 0 2px 0 #007052;
  }
</style>
