<script>
  import * as Highcharts from "highcharts";
  import "highcharts/modules/exporting";
  import { Chart } from "@highcharts/svelte";
  import Scroller from "../lib/Scroller.svelte";
  import ArticleText from "../lib/ArticleText.svelte";

  let options = {
    chart: {
      type: "pie",
    },
    title: {
      text: "An Example Pie Chart",
    },
    plotOptions: {
      pie: {
        allowPointSelect: true,
        dataLabels: [
          {
            enabled: true,
            distance: 20,
          },
          {
            enabled: true,
            distance: -40,
            format: "{point.percentage:.1f}%",
            style: {
              fontSize: "1.2em",
              textOutline: "none",
            },
            filter: {
              operator: ">",
              property: "percentage",
              value: 10,
            },
          },
        ],
      },
    },
    series: [
      {
        name: "Group",
        data: [
          {
            name: "Group 1",
            y: 151,
          },
          {
            name: "Group 2",
            sliced: true,
            selected: true,
            y: 180,
          },
          {
            name: "Group 3",
            y: 32,
          },
          {
            name: "Group 4",
            y: 103,
          },
          {
            name: "Group 5",
            y: 77,
          },
        ],
      },
    ],
  };
</script>

<div>
  <Scroller layout="right">
    {#snippet sticky()}
      <div class="chart">
        <Chart {options} highcharts={Highcharts} />
      </div>
      <p>
        Here's an example chart using
        <a href="https://www.highcharts.com/">Highcharts</a>!
      </p>
      <p>
        📈 <strong>Highcharts</strong> is a super-flexible library for creating
        all kinds of charts. See demos of different chart types
        <a href="https://www.highcharts.com/demo">here</a>.
      </p>
      <p>
        Since we're using Highcharts through Svelte, the syntax is a little
        different from what you might see in the demos. But all of Highcharts'
        functionality is available through the Highcharts for Svelte package.
      </p>
      <p>
        The configuration is done through the
        <code>options</code> json object passed to the chart, which you'll see in
        the source code for this template.
      </p>
      <p>
        Use the
        <a href="https://api.highcharts.com/highcharts/">API reference</a>
        to understand what each element in the <code>options</code> object does.
      </p>
    {/snippet}

    {#snippet scrolly()}
      <ArticleText>
        Wealth inequality in the U.S. are tied down to our historical roots and
        racial wealth gaps is a huge challenge for us to this day.
      </ArticleText>

      <ArticleText>
        We will focusing on Black-owned businesses and their access to loans and
        financial support shown in the <a href="https://blackwealthdata.org/"
          >Black Wealth Data Center</a
        >
      </ArticleText>

      <ArticleText>
        The data shown will be focused in <strong>Cumberland County, North Carolina </strong> 
      </ArticleText>

      <ArticleText>
        This project will try to answer this question: <br><br>
        
        <strong>“What are the key differences in business outcomes (e.g., revenue, profitability, employment) between Black-owned and white-owned businesses, and how much of that can be attributed to disparities in access to capital?”</strong>
      
    </ArticleText>
    {/snippet}
  </Scroller>
</div>

<style>
  .chart {
    width: 90%;
    margin: 0px auto;
  }
</style>
