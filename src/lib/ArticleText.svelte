<script>
  let { children } = $props();
</script>

<div class="article-text">
  <p>
    {@render children()}
  </p>
</div>

<style>
  .article-text {
    margin: 50vh auto;
    width: 50%;
    background-color: #623e2a;
    color: white;
    border: solid #553524 3px;
    border-radius: 20px;
    padding: 20px;
  }
</style>
