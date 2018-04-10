<template>
  <div>
    <Hero/>
    <ServiceList/>
    <Portfolio/>
    <About/>
    <Contact/>
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
