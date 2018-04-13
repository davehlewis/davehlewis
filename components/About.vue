<template>
  <section id="about" class="about bg-white p-8" @mouseover.stop="avatarDirection">
    <div class="about__image mb-4 md:mb-0 is-looking-right"><svg class="w-full h-auto" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16"><path fill="#6917A7" d="M1 16v-1h1v-2h1v-1h1v-1h1v-1h5v1h1v1h1v1h1v2h1v1z"/><path fill="#666" d="M11 16H4v-1h1v-1h1v-3h3v2h1v1h1z"/><path fill="none" stroke="#CCC" stroke-miterlimit="10" d="M2 15.5H1m11 0h-1m3 0h-1m0-1h-1m0-1h-1m0-1h-1m0-1H9m-5 4H3m0-1H2m3 0H4m0-1H3m3 0H5m0-1H4m2-1H5"/><path fill="#ECCCA3" d="M6 8h3v3H6z"/><path opacity=".2" fill="none" stroke="#000" stroke-miterlimit="10" d="M6.5 9v5m-1-4v5m-1-4v5m-1-4v3m4-4v4m1-4v3m2 0v1"/><path opacity=".2" fill="none" stroke="#FFF" stroke-miterlimit="10" d="M9.5 10v2m1-1v2m1-1v2m1-1v2m1 0v1"/><path fill="none" stroke="#190E04" stroke-miterlimit="10" d="M7 7.5H6"/><g class="frames"><path fill="#ECCCA3" d="M10 2H7v1H6v2h1v3H6v1h4z"/><path fill="#190E04" d="M11 0v1h-1v1H7v1H6v2h1v2H6V6H5V1h2V0z"/><path fill="none" stroke="#000" stroke-miterlimit="10" d="M9 4.5h1m-3 0h1"/><path opacity=".4" fill="#190E04" d="M7 7h1v1h2v1H7z"/><path opacity=".2" fill="none" stroke="#000" stroke-miterlimit="10" d="M7.5 2v1m-1 0v2m1 0v3.5H6"/><path fill="#ECCCA3" d="M10-8v-6H7v1H6v2h1v3z"/><path fill="#190E04" d="M10-16v2H7v1H6v2h1v2H6v-1H5v-5h2v-1z"/><path fill="none" stroke="#000" stroke-miterlimit="10" d="M9-12.5h1m-3 0h1"/><path opacity=".4" fill="#190E04" d="M7-9h3v1H7z"/><path opacity=".2" fill="none" stroke="#000" stroke-miterlimit="10" d="M7.5-14v1m-1 0v2m1 1v2m1.5.5H6"/><path fill="#ECCCA3" d="M7 26h3v-6H7v1H6v2h1z"/><path fill="#190E04" d="M6 23H5v-4h1v-1h5v1h-1v1H7v1H6v2"/><path fill="none" stroke="#190E04" stroke-miterlimit="10" d="M6.5 24v1"/><path fill="none" stroke="#000" stroke-miterlimit="10" d="M9 22.5h1m-3 0h1"/><path opacity=".4" fill="#190E04" d="M7 24h1v1h2v1H7z"/><path opacity=".2" fill="none" stroke="#000" stroke-miterlimit="10" d="M7.5 20v1m-1 0v2m1 0v3"/></g></svg></div>
    <div class="about__description flex flex-col justify-center">
      <h2 class="font-pixel text-2xl lg:text-3xl text-purple mb-2">Who am I?</h2>
      <p class="font-serif lg:text-lg leading-normal text-grey-darker mb-4">As you've probably figured out by now, I build websites and systems. I built my first website when I was 14. It was awful. I still have it, and no, you can't see it.</p>
      <p class="font-serif lg:text-lg leading-normal text-grey-darker mb-4">I've learned a lot since then, having worked in the industry for over 10 years. I've worked with a wide variety of different businesses, ranging from builders, to financial services companies, to charities.</p>
      <p class="font-serif lg:text-lg leading-normal text-grey-darker mb-4">I started out working in IT, building up a knowledge of systems, which still comes in handy. My passion though was in the area where creativity and logic meet - web development.</p>
      <p class="font-serif lg:text-lg leading-normal text-grey-darker mb-4">As well as building things digitally, I love to build real-life things too. I make things out of wood, design things in 3D, and subsequently 3d print them. I'm also a pretty good baker if I do say so myself.</p>
      <p class="font-serif lg:text-lg leading-normal text-grey-darker mb-4">I'm a proud dad of 1 little girl, living in Nantgarw in Wales.</p>
    </div>
  </section>
</template>

<script>
import _ from 'lodash'
export default {
  methods: {
    avatarDirection: _.debounce((event) => {
      const size = document.querySelector('#about').offsetHeight;
      const lookUp =  size / 3;
      const lookRight = size * 2 / 3;
      const y = event.clientY;
      const avatar = document.querySelector('#about .about__image');

      if (y <= lookUp) {
        avatar.classList.remove('is-looking-down', 'is-looking-right')
        avatar.classList.add('is-looking-up');
      } else if (y  > lookUp && y <= lookRight) {
        avatar.classList.remove('is-looking-down', 'is-looking-up')
        avatar.classList.add('is-looking-right');
      } else {
        avatar.classList.remove('is-looking-up', 'is-looking-right')
        avatar.classList.add('is-looking-down');
      }
    }, 200)
  }
}
</script>

<style>
  @media only screen and (min-width: 48em) {
    .about {
      display: grid;
      grid-template-columns: 2fr 3fr;
      grid-gap: 2rem;
    }
    .about__image.is-looking-right .frames {
      transform: translateY(0);
    }
    .about__image.is-looking-up .frames {
      transform: translateY(16px);
    }
    .about__image.is-looking-down .frames {
      transform: translateY(-16px);
    }
  }
  @media only screen and (min-width: 62em) {
    .about {
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-gap: 2rem;
    }
  }
</style>
