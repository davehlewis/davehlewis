<template>
  <section id="hero" class="hero container relative bg-black p-8 md:min-h-screen-70 lg:min-h-screen">
    <div class="hero__content flex flex-col justify-center my-8 md:my-0">
      <h1 class="font-serif mb-4 md:mb-8 text-white font-normal text-center md:text-left text-4xl md:text-5xl">Hi, I'm Dave Lewis</h1>
      <p class="text-white-50 text-2xl sm:text-3xl md:text-4xl text-center md:text-left font-serif">I'm a <strong class="font-normal text-white">Web Designer</strong> and <strong class="font-normal text-white">Front-End Developer</strong></p>
      <footer class="text-center md:text-left mt-8">
        <a href="#portfolio" class="inline-block mb-4 px-6 py-2 font-pixel text-xl lg:text-2xl text-white hover:text-black hover:bg-white no-underline uppercase border-white border-4" v-smooth-scroll>See my work</a>
        <SocialList class="justify-center md:justify-start"/>
      </footer>
    </div>
    <div class="hero__image flex items-center justify-center">
      <svg class="w-full max-w-sm block mx-auto" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 32"><path stroke="#F0F1F2" stroke-width="2" d="M12 31h5"/><path stroke="#493C2B" d="M12 30.5h4"/><path fill="#005784" d="M2 21h10v1h1v1h1v2h1v5h-3v-6H2z"/><path fill="#6917A7" d="M4 10v1H3v1H2v9h1v1h4v-1h1v-7h3v-2h-1v-1H8v-1H4z"/><path stroke="#CCC" d="M5 10.5h1m1 0h1m-4 1h1m1 0h1m1 0h1m-6 1h1m1 0h1m1 0h1m-5 2h1m1 0h1m1 0h1m-5 2h1m1 0h1m1 0h1m-5 2h1m1 0h1m1 0h1m-5 2h1m1 0h1m1 0h1m1-8h1m-8 1h1m1 0h1m1 0h1m-5 2h1m1 0h1m1 0h1m-5 2h1m1 0h1m1 0h1m-5 2h1m1 0h1m1 0h1m-3 2h1m1 0h1m1-8h1m1 0h1"/><path fill="#ECCCA3" d="M5 3v7h2V9h1V3z"/><g fill="#190E04"><path opacity=".4" d="M5 7v2h3V8H6V7z"/><path d="M6 1v1H4v7h1V4h1V3h2V2h1V1z"/></g><path class="eye" stroke="#000" d="M6 5.5h1"/><path fill="#337380" d="M2 24V11H0v13h1v2h10v-2z"/><path fill="#9D9D9D" d="M6 26v3H5v1H3v1h8v-1H9v-1H8v-3z"/><path d="M2 30h2v2H2zM6 30h2v2H6zM10 30h2v2h-2z"/><path stroke="#9D9D9D" d="M11.5 19v13M23.5 19v13"/><path stroke="#493C2B" d="M11 18.5h13"/><path fill="#9D9D9D" d="M21 18h3v-1h-1v-6h-1v6h-1z"/><path stroke="#000" d="M21.5 7v8M13 17.5h4"/><g opacity=".2"><path d="M22 11h1v6h1v15h-1V19h-1v-1h-1v-1h1zM7 1v3H6v5h1v1H5V9H4V2h2V1zM12 22h1v1h1v2h1v5h2v2h-5zM8 26h3v-5h-1v2H6v-1h1v-1H3v-8h1v-1h2v-1h2v-1H4v1H3v1H2v12H1v2h5v3H5v1H2v1h9v-1H9v-1H8z"/></g><path class="screen-light" fill="#FFF" opacity=".1" d="M8 21H7V1h3v1h2v1h2v1h2v1h2v1h2v1h1v8h-1v1h-2v1h-5v1h-2v1H9v1H8v1z"/><g class="frames"><path stroke="#ECCCA3" stroke-width="2" d="M14 16h2m-2-4h2m23 1v4m23-6h2m-2 3h2m23-3v3"/><g fill="#6917A7"><path d="M9 14v1h3v1h2v-4h-3v2zM34 14v1h1v1h3v-3h-1v-1h-2v2zM58 13v-2h4v2h-2v1h2v2h-3v-1h-2v-2zM81 15h5v-4h-5v4z"/></g><path stroke="#CCC" d="M34 11.5h1m0 1h1m22-1h3m-25 2h1m0 1h1m-3 0h1m0 1h1m24-3h1m-3 1h1m-2 1h1m1 0h1m-2 1h1m1 0h1m20-4h1m1 0h1m-4 1h1m1 0h1m1 0h1m-5 2h1m1 0h1m1 0h1m-4-1h1m1 0h1m-74-1h1m1 0h1m-2 1h1m-4 1h1m1 0h1m1 0h1m-2 1h1"/><g opacity=".25"><path stroke="#000" d="M9 14.5h2"/><path d="M12 12v1h1v1h1v-1h2v-2h-2v1zM40 15v2h-2v-1h-3v-1h-1v-2h1v1h1v1zM58 13v1h-1v1h2v1h3v-1h2v-2h-2v1h-2v-1zM88 13v1h-2v1h-5v-1h1v-1z"/></g><g opacity=".15"><path stroke="#FFF" d="M14 15.5h2m-4-1h2m-3-1h2m21-2h1m0 1h2M63.5 10v2m24-1v2"/><path fill="#FFF" d="M37 14h2v1h1v-2h-3z"/></g></g></svg>
    </div>
  </section>
</template>

<script>
import SocialList from '~/components/SocialList'
export default {
  components: {
    SocialList
  }
}
</script>


<style scoped>
  .hero {
    background-image: radial-gradient(circle at center, rgba(255,255,255,0.05) 0%, rgba(255,255,255,0) 60%);
  }

  .hero:before, .hero:after {
    content: '';
    display: block;
    background: #DFF5F9;
    transform-origin: 0 0;
    height: 1em;
    width: 50vw;
    position: absolute;
    bottom: 0;
  }

  .hero:before {
    left: 0;
    transform: skewY(5deg) translateY(-5em) scaleY(10);
  }

  .hero:after {
    right: 0;
    transform-origin: 100% 0;
    transform: skewY(-5deg) translateY(-5em) scaleY(10);
  }

  .hero__image svg .frames {
    animation: type 0.2s steps(4, end) infinite;
  }

  .hero__image svg .screen-light {
    animation: flicker 2s linear infinite;
  }

  .hero__image svg .eye {
    animation: blink 5s linear infinite;
  }

  @keyframes type {
    0% {
      transform: translateX(0);
    }
    100% {
      transform: translateX(-6rem);
    }
  }

  @keyframes flicker {
    0%, 19.999%, 22%, 62.999%, 64%, 64.999%, 70%, 100% {
      opacity: .1;
    }
    20%, 21.999%, 63%, 63.999%, 65%, 69.999% {
      opacity: 0.07;
    }
  }

  @keyframes blink {
    0%, 48%, 51%, 100% {
      opacity: 1;
    }
    50% {
      opacity: 0;
    }
  }

  @media only screen and (min-width: 48em) {
    .hero {
      background-image: radial-gradient(circle at 75% 50%, rgba(255,255,255,0.05) 0%, rgba(255,255,255,0) 60%);
      display: grid;
      grid-template-columns: 2fr 1fr;
      grid-gap: 2rem;
    }
    .hero__content {
      grid-column: 1;
    }
    .hero__image {
      grid-column: 2;
    }
  }

  @media only screen and (min-width: 62em) {
    .hero {
      grid-template-columns: 10em 1fr 1fr;
    }
    .hero__content {
      grid-column: 2;
    }
    .hero__image {
      grid-column: 3;
    }
  }
</style>
