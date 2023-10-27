<template>
  <div class="my-5 lg:h-[70vh] h-auto px-12">
    <section class="title">
      <h2 class="text-center font-semibold md:text-6xl text-4xl my-10">About</h2>
    </section>
    <section class="flex flex-col md:flex-row justify-center items-center">
      <div class="flex-1">
        <img src="../assets/hijab.jpg" alt="" class="grayscale lg:h-[55vh] md:h-[60vh] h-[30vh]" />
      </div>
      <div class="flex-1 md:px-5 animate__animated animate__fadeInTopLeft">
        <h2 class="font-semibold text-lg lg:text-2xl py-5">
          Welcome to Zain Amoire – Where Modesty Meets Modernity!
        </h2>
        <p class="leading-[1.55]">
          Step into a realm of elegance and grace at Zain Amoire. We specialize
          in curated collections of hijabs, palazzo pants, and veils, designed
          for the confident, modest woman of today.
        </p>
        <h2 class="font-semibold text-lg lg:text-2xl pt-3 ">Why Zain Amoire?</h2>
        <p v-for="q in quality" class="py-2"><span class=" font-semibold">{{ q.title }}</span>{{ q.body }}</p>
      </div>
    </section>
  </div>
</template>
<script>
export default {
  data() {
    return {
      quality: [
        {
          title: "🌟 Modest Fashion Mastery:",
          body: " Explore our expertly crafted hijabs, palazzo pants, and veils tailored to perfection.",
        },
        {
          title: "🌟 Premium Quality: ",
          body: "Luxurious fabrics and impeccable stitching for ultimate comfort and longevity.",
        },
        {
          title: "🌟 Chic Modesty: ",
          body: "Stay chic and on-trend with our contemporary, modest designs.",
        },
        {
          title: "🌟 Empowering Women:",
          body: " Celebrating your unique style while honoring traditions with grace.",
        },
      ],
    };
  },
};
</script>
