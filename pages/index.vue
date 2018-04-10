<template>
  <div>
    <Hero class="home-section"/>
    <ServiceList class="home-section"/>
    <Portfolio class="home-section"/>
    <About class="home-section"/>
    <Contact class="home-section"/>
  </div>
</template>

<script>
import Hero from '~/components/Hero'
import ServiceList from '~/components/ServiceList'
import Portfolio from '~/components/Portfolio'
import About from '~/components/About'
import Contact from '~/components/Contact'
export default {
  components: {
    Hero,
    ServiceList,
    Portfolio,
    About,
    Contact
  }
}
</script>

<style scoped>
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
