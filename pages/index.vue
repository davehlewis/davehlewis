<template>
  <div>
    <Hero/>
    <ServiceList/>
  </div>
</template>

<script>
import Hero from '~/components/Hero'
import ServiceList from '~/components/ServiceList'
export default {
  components: {
    Hero,
    ServiceList
  }
}
</script>
