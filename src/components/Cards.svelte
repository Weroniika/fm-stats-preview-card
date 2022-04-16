<script>
  import { cards } from "../data";
  import Card from "./Card.svelte";
</script>

<div class="cards">
  {#each cards as card}
    <Card {card} />
  {/each}
</div>

<style>
  .cards {
    display: grid;
    gap: 1.5rem;
  }

  @media (min-width: 48.625rem) {
    .cards {
      grid-auto-flow: column;
      max-width: 40ch;
    }
  }
</style>
