<section class="main-image">
  <div class="main-image__layer" />
  <picture>
    <source
      srcset="./images/image-header-desktop.jpg"
      media="(min-width: 778px)"
    />
    <img
      class="main-image__img"
      src="./images/image-header-mobile.jpg"
      alt="image header"
    />
  </picture>
</section>

<style>
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

  @media (min-width: 48.625rem) {
    .main-image {
      order: 1;
    }

    .main-image__img {
      min-width: 33.75rem;
      border-radius: 0 0.5rem 0.5rem 0;
    }
  }
</style>
