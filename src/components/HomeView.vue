<template>
  <div class="">
    <span
      class="border-2 border-black fixed bottom-10 right-1 p-2 rounded-full animate-bounce w rot"
      @click="scrollToTop"
      ><img src="@/assets/angle-up.png" class="w-5"
    /></span>
    <headerSection class="z-20" />
    <hero class="-z-10" />
    <about id="abt" />
    <products id="prod" />
    <feedback />
    <FAQ  id="faq"/>
    <footerSection id="contact" />
  </div>
</template>
<script>
import headerSection from "./headerSection.vue";
import hero from "./hero.vue";
import about from "./about.vue";
import products from "./products.vue";
import feedback from "./feedback.vue";
import FAQ from "./FAQ.vue";
import footerSection from "./footerSection.vue";
import AOS from 'aos';
import 'aos/dist/aos.css'; // Import AOS styles

export default {
  components: {
    headerSection,
    hero,
    about,
    products,
    feedback,
    FAQ,
    footerSection,
  },
  methods:{
    scrollToTop(){
      window.scrollTo(0,0)
    }
  },
  mounted(){
    AOS.init({
      duration: 500, // Animation duration
      easing: 'ease-in-out', // Easing option
     // Whether animation should happen only once
    });
  }
};
</script>
<style>
.rot {
  transform: rotateY(30deg);
}
</style>
