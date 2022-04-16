<script>
  export let card;
</script>

<div class="card">
  <h2 class="card__title">{card.stat}</h2>
  <h3 class="card__content">{card.content}</h3>
</div>

<style>
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
    .card__content {
      margin-top: 0.125rem;
    }
  }
</style>
