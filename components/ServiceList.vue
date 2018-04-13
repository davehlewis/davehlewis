<template>
  <section id="services" class="relative p-4 md:p8 flex items-center bg-blue-lightest">
    <div class="services-list mx-auto md:max-w-2xl">
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
        description: 'Using the latest technologies, I can make your website work well for any user, on any device. Interactivity usually only found on bigger sites is within reach of any business.',
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

<style>
  #services {
    background-image: linear-gradient(#DFF5F9, white);
    /*background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 30 30"><path fill="%23FFF" d="M0 20h30v10H0z"/><path fill="%23DFF5F9" d="M0 10v10l15 1 15-1V10z"/><path fill="%239DDFED" d="M0 0v10l15 1 15-1V0z"/></svg>');*/
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }

  @media only screen and (min-width: 48em) {
    .services-list {
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-gap: 2rem;
    }
  }

  @media only screen and (min-width: 62em) {
    .services-list {
      grid-gap: 6rem;
    }
  }
</style>
