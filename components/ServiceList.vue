<template>
  <section id="services" class="relative bg-blue-lightest p-4 md:p8">
    <div class="services-list mx-auto md:max-w-xl">
      <ServiceListItem v-for="service in services" :key="service.title" :title="service.title" :icon="service.icon">
        {{ service.description }}
      </ServiceListItem>
    </div>
  </section>
</template>

<script>
import ServiceListItem from '~/components/ServiceListItem'
export default {
  data: () => ({
    services: [
      {
        title: 'Web & UI Design',
        description: 'Specialising in great user experience, I work with all types of clients to offer great design. My priority is creating a site that works best for users and conveys your companies values.',
        icon: ''
      },
      {
        title: 'Web Development',
        description: 'I use the latest tools and practises to ensure your website is fully responsive, runs quickly, and has great user functionality. Interactivity usually only found on bigger sites is within reach of any business.',
        icon: ''
      },
      {
        title: 'Email Design & Coding',
        description: 'A great email design can be the key to a conversion. Given the number of platforms now in use, across a range of devices, quality coding is more important now than ever.',
        icon: ''
      },
      {
        title: 'Website Speed',
        description: 'Page Speed is now critically important for SEO and user experience. Speed can depend on a variety of factors. I can audit and takes steps to improve performance for your site.',
        icon: ''
      },
    ]
  }),
  components: {
    ServiceListItem
  }
}
</script>

<style scoped>
  @media only screen and (min-width: 48em) {
    .services-list {
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-gap: 2rem;
    }
  }
</style>
