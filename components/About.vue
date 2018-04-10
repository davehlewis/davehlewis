<template>
  <section id="about" class="about bg-grey-lighter p-8">
    <div class="about__image"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16"><path fill="#948068" d="M8 8h2v1H8z"/><path fill="#726457" d="M8 9H7V7h1v2z"/><path fill="#190E04" d="M7 8H6V6H5V1h2V0h4v1h-1v1H7v1H6v2h1v3z"/><path fill="#BAA384" d="M8 7H7V5h1v2zM7 3H6v2h1V3zm1-1H7v1h1V2zM7 8H6v3h1V8z"/><path fill="#ECCCA3" d="M10 2v2H9v1h1v3H8V4H7V3h1V2h2zM9 9H7v2h2V9z"/><path d="M8 5H7V4h1v1zm2-1H9v1h1V4z"/><path fill="#666" d="M9 13h1v2h1v1H5v-1h1v-1h1v1h1v-1h1z"/><path fill="#4D4D4D" d="M6 11h3v3H8v1H7v-1H6v-3zm5 3h-1v1h1v-1zm-6 1h1v-1H5v1zm0 0H4v1h1v-1z"/><path fill="#3E0E62" d="M5 10h1v1H5z"/><path fill="#653E81" d="M4 11h1v1H4z"/><path fill="#8745B9" d="M3 12h1v1H3v-1zm-1 2h1v-1H2v1z"/><path fill="#6917A7" d="M5 12h1v1H5v-1zm-1 2h1v-1H4v1zm-1 1h1v-1H3v1zm-1 1h1v-1H2v1zm7-5h1v-1H9v1z"/><path fill="#B378E1" d="M11 12h1v1h-1v-1zm-1 0h1v-1h-1v1zm2 2h1v-1h-1v1z"/><path fill="#801ECD" d="M9 12h1v1H9v-1zm1 2h1v-1h-1v1zm1 1h1v-1h-1v1zm1 1h1v-1h-1v1z"/><path fill="#E6E6E6" d="M10 12H9v-1h1v1zm1 0h-1v1h1v-1zm1 1h-1v1h1v-1zm1 1h-1v1h1v-1zm1 1h-1v1h1v-1z"/><path fill="#B3B3B3" d="M11 15h1v1h-1z"/><path fill="#CCC" d="M6 12H5v-1h1v1zm-1 0H4v1h1v-1zm-1 1H3v1h1v-1zm-1 1H2v1h1v-1zm-1 1H1v1h1v-1zm4-2H5v1h1v-1zm-1 1H4v1h1v-1zm-1 1H3v1h1v-1z"/></svg></div>
    <div class="about__description">
      <h2>Who am I?</h2>
      <p>As you've probably figured out by now, I build websites and systems. I built my first website when I was 14. It was awful. I still have it, and no you can't see it.</p>
      <p>I've learned a lot having worked in the industry for over 10 years now. Along the way, I've worked with a wide variety of different businesses and people. These range from builders, to financial services companies, to charities; from bi,g multinational companies to individuals just starting out with their big idea.</p>
      <p>I started out working in IT support, building up a great knowledge of systems, which still comes in handy with my work today. My passion though was in the wonderful area where creativity and logic meet - web development. Since then, I have worked in full-stack roles, but now am moving more towards front-end development and wedsite design as a whole.</p>
      <p>Nowadays I create static sites using Hugo and Nuxt, and utilising Vue and Angular for web applications. Unlike many developers, I adore CSS, and love how things are progressing in this area. I also dabble in Mobile App design, either natively or using NativeScript.</p>
      <p>As well as building things digitally, I love to build real-life things too. I love to make things out of wood, to design things in 3D, and subsequently 3d print them. I'm also a pretty good baker if I do say so myself.</p>
      <p>I'm a proud dad of 1 little girl, living in Nantgarw in Wales.</p>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>
  @media only screen and (min-width: 48em) {
    .about {
      display: grid;
      grid-template-columns: 1fr 2fr;
      grid-gap: 2rem;
    }
  }

</style>
