<template>
  <div class="service flex flex-row items-end mb-4">
    <div class="service__icon bg-blue w-16 h-16 md:w-24 md:h-24 text-white"></div>
    <div class="service__content flex-1 bg-white p-4 border-2 border-blue-light">
      <h2 class="font-pixel text-xl mb-4">{{ title }}</h2>
      <p class="my-auto font-serif text-grey-darker"><slot></slot></p>
    </div>
  </div>
</template>

<script>
export default {
  props: ['title', 'icon'],
}
</script>

<style>
  .service:nth-child(odd) {
    flex-direction: row-reverse;
    align-items: flex-start;
  }
</style>
