<template>
  <ul class="social-list list-reset flex flex-row">
    <li><a class="inline-block h-12 p-2 text-white-50 hover:text-white" v-for="social in sociallinks" :key="social.title" :href="social.url" :title="social.title" :aria-label="social.title" v-html="social.icon"></a></li>
  </ul>
</template>

<script>
export default {
  data: () => ({
    sociallinks: [
      {
        title: 'LinkedIn',
        url: 'https://www.linkedin.com/in/davehlewis',
        icon: '<svg class="fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M22 3V2h-1V1H3v1H2v1H1v18h1v1h1v1h18v-1h1v-1h1V3h-1zM8 21H5V10h3v11zM8 8H5V5h3v3zm11 13h-3v-8h-3v8h-3V10h8v1h1v10z"/></svg>'
      },
      {
        title: 'Twitter',
        url: 'https://twitter.com/davehlewis',
        icon: '<svg class="fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M1 3h1v1h1v1h1v1h1v1h2v1h3v1h2V6h1V4h2V3h3v1h2v1h1V4h2v1h-1v1h1v1h-1v1h-1v5h-1v2h-1v2h-1v1h-1v1h-1v1h-2v1h-3v1H5v-1H1v-1h4v-1h2v-2H4v-1H3v-1h1v-1H3v-1H2v-1H1v-2h2V9H2V8H1z"/></svg>'
      },
      {
        title: 'Github',
        url: 'https://github.com/davehlewis/',
        icon: '<svg class="fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M6 18h1v1h2v2H7v-1H6v-1H5v-1H4v-1h2v1zm15-9V7h-1V6h-1V5h-1V4h-1V3h-2V2H9v1H7v1H6v1H5v1H4v1H3v2H2v6h1v2h1v-1h2v1h1v1h2v-1H8v-1H7v-1H6v-1H5v-4h1V9h1V6h1v1h1v1h6V7h1V6h1v3h1v1h1v4h-1v1h-1v1h-1v1h-1v4h2v-1h1v-1h1v-1h1v-1h1v-2h1V9h-1z"/></svg>'
      },
      {
        title: 'Codepen',
        url: 'https://codepen.io/davehlewis/',
        icon: '<svg class="fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M9 9h2v1h-1v1H8v-1h1V9zm-4 2v2h3v-2H5zm9-1v1h2v-1h-1V9h-2v1h1zm2 1v2h3v-2h-3zm8-3v8h-1v1h-1v1h-2v1h-1v1h-1v1h-2v1h-2v1h-1v1h-2v-1h-1v-1H8v-1H6v-1H5v-1H4v-1H2v-1H1v-1H0V8h1V7h1V6h2V5h1V4h2V3h1V2h2V1h1V0h2v1h1v1h2v1h1v1h2v1h1v1h2v1h1v1h1zm-1 2h-2v1h-2v-1h1V9h2V8h-1V7h-2V6h-1V5h-2V4h-1V3h-2v6h-2V3H9v1H8v1H6v1H5v1H3v1H2v1h2v1h1v1H3v-1H1v4h2v-1h2v1H4v1H2v1h1v1h2v1h1v1h1v1h2v1h2v-5h-1v-1H9v-1H8v-1h2v1h1v1h2v-1h1v-1h2v1h-1v1h-1v1h-1v5h2v-1h2v-1h1v-1h1v-1h2v-1h1v-1h-2v-1h-1v-1h2v1h2v-4z"/></svg>'
      }
    ]
  }),
}
</script>

<style>
  svg {
    height: 100%;
  }
</style>
