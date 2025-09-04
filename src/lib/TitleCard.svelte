<script>
  let { title, subtitle } = $props();
</script>

<div class="title-card">
  <div class="content">
    <h1>{title}</h1>
    <p>{subtitle}</p>
  </div>
</div>

<style>
  .title-card {
    background-color: ##623e2a;
    background-color: transparent;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 2rem;
    box-sizing: fill;
    font-family: "Inter", sans-serif;
  }

  .content {
    max-width: 900px;
    background-color: #623e2a;
    padding: 2rem;
    border-radius: 2rem;
  }

  h1 {
    font-size: 3rem;
    margin: 0;
    color: white;
    text-shadow: 1px 1px 0 #3d2111;
  }

  p {
    font-size: 1.3rem;
    color: #f7f5eb;
    margin-top: 1rem;
  }

  @media (max-width: 600px) {
    h1 {
      font-size: 2.2rem;
    }

    p {
      font-size: 1.1rem;
    }
  }
</style>
