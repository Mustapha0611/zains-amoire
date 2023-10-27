<script>
import preloader from "./components/preloader.vue";
import HomeView from "./components/HomeView.vue";
import hero from "./components/hero.vue";
import 'animate.css';
import aos from 'aos';
export default {
  components: {
    preloader,
    HomeView,
    hero
  },
  mounted() {
    const randomNum = Math.random() * 5;
    setTimeout(() => {
      this.isLoading = false;
    }, this.loadingTime + randomNum);
    console.log(randomNum);
    aos.init()
  },
  data() {
    return {
      isLoading: true,
      loadingTime: 2000,
    };
  },
};
</script>

<template>
  <div>
    <Transition
      name="custom-classes"
      enter-active-class=""
      leave-active-class="animate__animated animate__zoomOut animate__faster"
    >
      <preloader v-if="isLoading" />
      <HomeView v-else />
    </Transition>
  </div>
</template>
<style>
 html{
  scroll-behavior: smooth;
 }
</style>