<script>
  import Cards from "./components/Cards.svelte";
  import Content from "./components/Content.svelte";
  import Image from "./components/Image.svelte";
</script>

<main class="main">
  <Image />
  <Content />
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
  @media (min-width: 48.625rem) {
    .main {
      grid-auto-flow: column;
      grid-template-columns: 1fr 1fr;
      padding: 11.0625rem 10.3125rem;
      gap: unset;
      justify-items: unset;
    }
  }
</style>
