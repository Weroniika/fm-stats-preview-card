<script>
  import Cards from "./Cards.svelte";
</script>

<section class="main-content">
  <h1 class="main-content__title">
    Get
    <span class="main-content__title--violet">insights</span>
    that help your business grow.
  </h1>
  <p class="main-content__text">
    Discover the benefits of data analytics and make better decisions regarding
    revenue, customer experience, and overall efficiency.
  </p>
  <Cards />
</section>

<style>
  .main-content {
    background-color: var(--color-dark-desaturated-blue);
    padding: 2.5rem 1.9688rem 2rem;
    text-align: center;
    border-radius: 0 0 0.5rem 0.5rem;
    display: grid;
    justify-content: center;
  }
  .main-content__title {
    font-weight: 700;
    font-size: 1.75rem;
    line-height: 2rem;
  }
  .main-content__text {
    color: var(--color-white-paragraphs);
    line-height: 1.5625rem;
    margin: 1.1rem 0 2rem;
  }

  .main-content__title--violet {
    color: var(--color-violet);
  }

  @media (min-width: 48.625rem) {
    .main-content {
      text-align: left;
      padding: 4.4375rem 5.9375rem 3.6875rem 4.5rem;
      border-radius: 0.5rem 0 0 0.5rem;
      align-items: start;
    }
    .main-content__title {
      min-width: 18ch;
      max-width: 20ch;
      font-size: 2.25rem;
      line-height: 2.75rem;
    }
    .main-content__text {
      max-width: 40ch;
      margin: 1.1rem 0 3rem;
    }
  }
</style>
