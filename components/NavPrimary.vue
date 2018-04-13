<template>
  <nav class="fixed z-10 pin-t pin-l">
    <button class="inline-block nav__toggle w-16 h-16 bg-black" @click="navVisible = !navVisible" aria-label="Show Navigation"><span></span></button>
    <ul class="nav__list list-reset opacity mt-2 bg-black border-4 border-white py-2 px-4" :class="{ 'is-shown': navVisible }">
      <li><a href="#hero" v-smooth-scroll>Home</a></li>
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


<style>
  .nav__toggle {
    opacity: 0.6;
    outline: none;
    position: relative;
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
    left: 50%;
    width: 2.5rem;
    height: 0.25rem;
  }

  .nav__toggle span:before,
  .nav__toggle span:after {
    content: '';
  }

  .nav__toggle span {
    top: 50%;
    transform: translate(-50%, -50%);
  }

  .nav__toggle span:before {
    transform: translate(-50%, -0.75rem);
  }

  .nav__toggle span:after {
    transform: translate(-50%, 0.75rem);
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
</style>

