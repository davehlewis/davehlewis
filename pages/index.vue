<template>
  <div>
    <Hero/>
    <ServiceList/>
    <Portfolio/>
    <About/>
  </div>
</template>

<script>
import Hero from '~/components/Hero'
import ServiceList from '~/components/ServiceList'
import Portfolio from '~/components/Portfolio'
import About from '~/components/About'
export default {
  components: {
    Hero,
    ServiceList,
    Portfolio,
    About
  }
}
</script>
