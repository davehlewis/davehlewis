<template>
  <nav class="fixed z-10 pin-t pin-l lg:pin-none p-4">
    <button class="nav__toggle lg:hidden" @click="navVisible = !navVisible" aria-label="Show Navigation"><span></span></button>
    <ul class="nav__list list-reset opacity mt-2 lg:mt-0 bg-black lg:bg-transparent border-4 lg:border-0 border-white py-2 px-4 lg:p-0" :class="{ 'is-shown': navVisible }">
      <li><a href="#hero" v-smooth-scroll></a></li>
      <li><a href="#services" v-smooth-scroll class="block text-xl font-pixel pl-6 py-1 text-white-50 hover:text-white no-underline">Services</a></li>
      <li><a href="#portfolio" v-smooth-scroll class="block text-xl font-pixel pl-6 py-1 text-white-50 hover:text-white no-underline">My Work</a></li>
      <li><a href="#about" v-smooth-scroll class="block text-xl font-pixel pl-6 py-1 text-white-50 hover:text-white no-underline">Who Am I?</a></li>
      <li><a href="#contact" v-smooth-scroll class="block text-xl font-pixel pl-6 py-1 text-white-50 hover:text-white no-underline">Get in Touch</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  data: () => ({
    navVisible: false
  })
}
</script>


<style scoped>
  .nav__toggle {
    height: 2rem;
    opacity: 0.6;
    outline: none;
    position: relative;
    width: 2.5rem;
  }

  .nav__toggle:hover,
  .nav__toggle:focus {
    opacity: 1;
  }

  .nav__toggle span,
  .nav__toggle span:before,
  .nav__toggle span:after {
    background: white;
    display: block;
    position: absolute;
    width: 100%;
    height: 0.25rem;
  }

  .nav__toggle span:before,
  .nav__toggle span:after {
    content: '';
  }

  .nav__toggle span {
    top: 50%;
    transform: translateY(-50%);
  }

  .nav__toggle span:before {
    transform: translateY(-0.75rem);
  }

  .nav__toggle span:after {
    transform: translateY(0.75rem);
  }

  .nav__list {
    transform: translatex(-100vw);
  }

  .nav__list.is-shown {
    transform: translatex(0);
  }
  
  .nav__list li a {
    mix-blend-mode: difference;
  }

  @media only screen and (min-width: 62em) {
    nav {
      top: 50%;
      transform: translateY(-50%);
    }
    .nav__list {
      transform: translatex(0);
    }
  }
</style>

