<template>
  <div class="site">
    <NavPrimary/>
    <nuxt/>
  </div>
</template>

<script>
  import NavPrimary from '~/components/Navprimary'
  export default {
    components: {
      NavPrimary
    }
  }
</script>

