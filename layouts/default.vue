<template>
  <div class="site">
    <NavPrimary/>
    <nuxt/>
  </div>
</template>

<script>
  import NavPrimary from '~/components/NavPrimary'
  export default {
    components: {
      NavPrimary
    }
  }
</script>

