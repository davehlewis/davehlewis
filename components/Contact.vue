<template>
  <section id="contact" class="contact p-8 bg-purple-dark text-purple-lightest">
    <h2 class="font-pixel text-2xl lg:text-3xl text-purple-lightest text-center mb-4">Get in touch</h2>
    <p class="font-serif text-lg lg:text-xl text-purple-lighter text-center mb-8">Please use the form below, or call me on <a href="tel:+447802636853" class="text-purple-lightest no-underline">07802 636853</a></p>
    <ContactForm class="contact__form max-w-lg mx-auto" />
  </section>
</template>

<script>
import ContactForm from '~/components/ContactForm'
export default {
  components: {
    ContactForm
  }
}
</script>
