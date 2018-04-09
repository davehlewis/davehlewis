<template>
  <ul class="social-list">
    <li><a v-for="social in sociallinks" :key="social" :href="social.url" :title="social.title" :aria-label="social.title">{{ social.title }}</a></li>
  </ul>
</template>

<script>
export default {
  data: () => ({
    sociallinks: [
      {
        title: 'LinkedIn',
        url: 'https://www.linkedin.com/in/davehlewis',
        icon: ''
      },
      {
        title: 'Twitter',
        url: 'https://twitter.com/davehlewis',
        icon: ''
      },
      {
        title: 'Github',
        url: 'https://github.com/davehlewis/',
        icon: ''
      },
      {
        title: 'Codepen',
        url: 'https://codepen.io/davehlewis/',
        icon: ''
      }
    ]
  })
}
</script>

<style>

</style>
