<template>
  <div>
    <Hero class="home-section"/>
  </div>
</template>

<script>
import Hero from '~/components/Hero'
export default {
  components: {
    Hero
  }
}
</script>

<style>
  .home-section {
    padding: 4rem 2rem;
  }
  @media only screen and (min-width: 62em) {
    .home-section {
      padding: 6rem 4rem;
      min-height: 80vh;
    }
  }
</style>
