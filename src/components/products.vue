<template>
  <div class="px-10">
    <section class="title">
      <h2 class="text-center font-semibold md:text-6xl text-4xl my-10" data-aos="fade-up" >
        Store
      </h2>
    </section>
    <section class="flex flex-col flex-wrap md:flex-row justify-center gap-10 items-center">
      <div class=" shadow-xl md:w-[320px] w-[90%] h-[50vh] border-2 border-gray-100 rounded-lg hover:scale-105 transition-all overflow-hidden" v-for="prod in products" data-aos="fade-up">
        <img :src="prod.img" alt="" class="w-full h-[40vh] grayscale  hover:scale-105 transition-all overflow-hidden" data-aos="zoom-in"
        data-aos-delay="300">
        <span class="text-2xl p-5 font-semibold block">{{ prod.title }}</span>
    </div>
    </section>
  </div>
</template>
<script>
import hijab from "../assets/hijab.png";
import wrapskirt from "../assets/wrapskirt.png";
import wraptop from "../assets/wraptop.png";
import trouser from "../assets/trouser.png";
import skirts from "../assets/skirts.png";
import gowns from "../assets/gowns.png"
import palazzo from "../assets/palazzo.png";
import viel from "../assets/viel.png";

export default {
  data() {
    return {
      products: [
        {
          title: "Hijab",
          img: hijab,
        },
        {
          title: "Wrap Skirt",
          img: wrapskirt,
        },
        {
          title: "Palazzo",
          img: palazzo,
        },
        {
          title: "Veil",
          img: viel,
        },
        {
          title: "Wrap Top",
          img: wraptop,
        },
        {
          title: "Gowns",
          img: gowns,
        },
        {
          title: "Trousers",
          img: trouser,
        },
        {
          title: "Skirt",
          img: skirts,
        },
      ],
    };
  },
};
</script>
