<template>
  <section id="portfolio" class="portfolio bg-buff-lighter pad-8">
    <h2 class="font-pixel text-2xl lg:text-3xl text-buff-darkest text-center mb-4">My Work</h2>
    <p class="font-serif text-lg lg:text-xl text-buff-darker text-center mb-8">Below are a few examples of my work</p>
    <PortfolioPreview class="hidden lg:block" />
    <PortfolioList :examples="examples" />
  </section>
</template>

<script>
import PortfolioData from "~/data/portfolio.json"
import PortfolioPreview from '~/components/PortfolioPreview'
import PortfolioList from '~/components/PortfolioList'
import PortfolioItem from '~/components/PortfolioItem'
export default {
  data: () => ({
    examples: PortfolioData
  }),
  components: {
    PortfolioPreview,
    PortfolioList,
    PortfolioItem
  }
}
</script>

<style>
  @media only screen and (min-width: 62em) {
    /*.portfolio {
      display: grid;
      grid-template-columns: 1fr 2fr;
      grid-gap: 2rem;
    }*/
  }
</style>
