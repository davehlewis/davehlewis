<template>
  <section id="services">
    <ServiceListItem v-for="service in services" :key="service" :title="service.title" :icon="service.icon">
      {{ description }}
    </ServiceListItem>
  </section>
</template>

<script>
import ServiceListItem from '~/components/ServiceListItem'
export default {
  data: () => ({
    services: [
      {
        title: 'Web &amp; UI Design',
        description: '',
        icon: ''
      },
      {
        title: 'Web Development',
        description: '',
        icon: ''
      },
      {
        title: 'Email Design &amp; Coding',
        description: '',
        icon: ''
      },
      {
        title: 'Website Speed',
        description: '',
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

</style>
