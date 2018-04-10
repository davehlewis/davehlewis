<template>
  <div class="portfolio-list">
    <PortfolioListItem class="relative overflow-hidden" v-for="example in examples" :key="example.name">
      <img class="portfolio-item__thumb" :src="example.thumbnail" :alt="example.description">
      <div class="portfolio-item__content bg-buff-darker absolute pin-t pin-l w-full h-full flex flex-col justify-center p-8">
        <h3 class="font-pixel text-xl text-buff-lightest mb-4">{{ example.name }}</h3>
        <p class="font-serif text-lg text-buff-light">{{ example.description }}</p>
      </div>
    </PortfolioListItem>
  </div>
</template>

<script>
import PortfolioListItem from '~/components/PortfolioListItem'
export default {
  props: {
    examples: Array
  },
  components: {
    PortfolioListItem
  }
}
</script>

<style>
  .portfolio-list {
    display: grid;
    grid-gap: 0.25rem;
    justify-items: stretch;
  }

  .portfolio-item {
    min-height: 12rem;
  }

  .portfolio-item__thumb {
    object-fit: cover;
    height: 15rem;
    width: 100%;
  }

  .portfolio-item__content {
    transform: translateY(100vw);
    transition: transform 0.4s ease-in-out;
  }

  .portfolio-item:hover .portfolio-item__content {
    transform: translateY(0);
  }

  @media only screen and (min-width: 36em) and (max-width: 75em) {
    .portfolio-list {
      grid-template-columns: repeat(4, 1fr);
    }
    .portfolio-item:nth-child(3n+1) {
      grid-column: 2 / span 2;
    }
    .portfolio-item:nth-child(3n+2) {
      grid-column: 1 / span 2;
    }
    .portfolio-item:nth-child(3n+3) {
      grid-column: 3 / span 2;
    }
  }

  @media only screen and (min-width: 75em) {
    .portfolio-list {
      grid-template-columns: repeat(6, 1fr);
    }
    .portfolio-item:nth-child(5n+1) {
      grid-column: 2 / span 2;
    }
    .portfolio-item:nth-child(5n+2) {
      grid-column: 4 / span 2;
    }
    .portfolio-item:nth-child(5n+3) {
      grid-column: 1 / span 2;
    }
    .portfolio-item:nth-child(5n+4) {
      grid-column: 3 / span 2;
    }
    .portfolio-item:nth-child(5n+5) {
      grid-column: 5 / span 2;
    }
  }
</style>
