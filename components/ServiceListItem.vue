<template>
  <div class="service">
    <h2>{{ title }}</h2>
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: ['title', 'icon'],
}
</script>

<style>

</style>
