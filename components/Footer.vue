<template>
  <footer class="bg-black p-6">
    <p class="text-center font-pixel text-lg mb-8">
      <a href="#hero" v-smooth-scroll class="text-grey hover:text-grey-lightest no-underline">Back to Top</a>
    </p>
    <SocialList class="justify-center mb-8" />
    <p class="text-center text-grey font-serif">Copyright &copy; {{ year }} David Lewis</p>
  </footer>
</template>

<script>
import SocialList from '~/components/SocialList'
export default {
  data: () => ({
    year: (new Date()).getFullYear()
  }),
  components: {
    SocialList
  }
}
</script>
