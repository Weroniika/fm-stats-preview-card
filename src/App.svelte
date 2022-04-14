<main class="main">
  <section class="main-image">
    <div class="main-image__layer" />
    <picture>
      <source
        srcset="/images/image-header-desktop.jpg"
        media="(min-width: 778px)"
      />
      <img
        class="main-image__img"
        src="/images/image-header-mobile.jpg"
        alt="image header"
      />
    </picture>
  </section>
  <section class="main-content">
    <h1 class="main-content__title">
      Get
      <span class="main-content__title--violet">insights</span>
      that help your business grow.
    </h1>
    <p class="main-content__text">
      Discover the benefits of data analytics and make better decisions
      regarding revenue, customer experience, and overall efficiency.
    </p>
    <article class="cards">
      <div class="card">
        <h2 class="card__title">10k+</h2>
        <h3 class="card__content">companies</h3>
      </div>
      <div class="card">
        <h2 class="card__title">314</h2>
        <h3 class="card__content">templates</h3>
      </div>
      <div class="card">
        <h2 class="card__title">12m+</h2>
        <h3 class="card__content">queries</h3>
      </div>
    </article>
  </section>
</main>

<style>
  .main {
    min-height: 100vh;
    display: grid;
    background-color: var(--color-dark-blue);
    padding: 5.5rem 1.5rem;
    align-content: start;
    justify-items: center;
  }
  .main-image {
    position: relative;
    width: 100%;
  }
  .main-image__layer {
    width: 100%;
    height: 100%;
    position: absolute;
    left: 0;
    top: 0;
    background-color: var(--color-violet);
    z-index: 11;
    mix-blend-mode: multiply;
    opacity: 0.95;
  }
  .main-image__img {
    border-radius: 0.5rem 0.5rem 0 0;
    width: 100%;
    height: 100%;
    min-width: 20.4375rem;
    object-fit: cover;
  }
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

  .cards {
    display: grid;
    gap: 1.5rem;
  }
  .card__title {
    font-weight: 700;
    font-size: 1.5rem;
    line-height: 1.8125rem;
  }

  .card__content {
    font-weight: 400;
    font-size: 0.75rem;
    line-height: 1.5625rem;
    letter-spacing: 0.0625rem;
    text-transform: uppercase;
    color: var(--color-white-headings);
    mix-blend-mode: normal;
    opacity: 0.6;
  }

  @media (min-width: 48.625rem) {
    .main {
      grid-auto-flow: column;
      grid-template-columns: 1fr 1fr;
      padding: 11.0625rem 10.3125rem;
      gap: unset;
      justify-items: unset;
    }

    .main-image {
      order: 1;
    }
    .main-image__img {
      min-width: 33.75rem;
      border-radius: 0 0.5rem 0.5rem 0;
    }
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
    .cards {
      grid-auto-flow: column;
      max-width: 40ch;
    }
    .card__content {
      margin-top: 0.125rem;
    }
  }
</style>
