<template>
  <div class="site">
    <NavPrimary/>
    <nuxt/>
    <Footer/>
  </div>
</template>

<script>
  import NavPrimary from '~/components/NavPrimary'
  import Footer from '~/components/Footer'
  export default {
    components: {
      NavPrimary,
      Footer
    }
  }
</script>

