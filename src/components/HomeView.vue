<template>
  <div class="">
    <span
      class="border-2 border-black fixed bottom-10 right-2 p-5 rounded-full animate-bounce w rot"
      @click="scrollToTop"
      ><img src="@/assets/Angle-up.png" class="w-5"
    /></span>
    <headerSection class="z-20" />
    <hero class="z-10" />
    <about id="abt" />
    <products id="prod" />
    <feedback />
    <FAQ />
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
  }
};
</script>
<style>
.rot {
  transform: rotateY(30deg);
}
</style>
