<template>
  <form action="" class="contact__form">
    <div class="border-4 border-white py-4 px-6 mb-4">
      <label class="block font-pixel uppercase text-purple-lighter mb-2 px-2" for="contact-name">Your Name</label>
      <input class="text-xl font-serif w-full bg-purple-darker px-4 py-3 text-white" type="text" name="contact-name" id="contact-name">
    </div>
    <div class="border-4 border-white py-4 px-6 mb-4">
      <label class="block font-pixel uppercase text-purple-lighter mb-2 px-2" for="contact-email">Your Email</label>
      <input class="text-xl font-serif w-full bg-purple-darker px-4 py-3 text-white" type="email" name="contact-email" id="contact-email">
    </div>
    <div class="border-4 border-white py-4 px-6 mb-4">
      <label class="block font-pixel uppercase text-purple-lighter mb-4 px-2">What do you need?</label>
      <p class="mb-2" v-for="type in types" :key="type.value">
        <input class="hidden" type="radio" name="contact__what" :value="type.value" :id="'contact__what--' + type.value" :checked="type.checked">
        <label class="pl-8 font-pixel text-xl hover:text-white" :for="'contact__what--' + type.value">{{ type.text }}</label>
      </p>
    </div>
    <div class="border-4 border-white py-4 px-6 mb-4">
      <label class="block font-pixel uppercase text-purple-lighter mb-2 px-2" for="contact-message">Message</label>
      <textarea class="text-xl font-serif w-full bg-purple-darker px-4 py-3 text-white" name="contact-message" id="contact-message" cols="30" rows="4"></textarea>
    </div>
    <button class="inline-block mb-4 px-6 py-2 font-pixel text-xl lg:text-2xl text-white hover:text-purple hover:bg-white no-underline uppercase border-white border-4">Send</button>
  </form>
</template>

<script>
export default {
  data: () => ({
    types: [
      {value:'project', text:'Web/Design Project', checked: true},
      {value:'job', text:'Job Enquiry'},
      {value:'other', text:'Something Else'}
    ]
  })
}
</script>

<style scoped>
  input:focus, textarea:focus {
    outline: 4px solid #C3A2DC;
  }
</style>
