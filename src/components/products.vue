<template>
  <div class="px-10">
    <section class="title">
      <h2 class="text-center font-semibold md:text-6xl text-4xl my-10" data-aos="fade-up" >
        Store
      </h2>
    </section>
    <section class="flex flex-col flex-wrap md:flex-row justify-center gap-10 items-center">
      <div class=" shadow-xl md:w-[320px] w-[90%] h-[50vh] border-2 border-gray-100 rounded-lg hover:scale-105 transition-all overflow-hidden" v-for="prod in products" data-aos="fade-up">
        <img :src="prod.img" alt="" class="w-full h-[40vh] grayscale  hover:scale-105 transition-all overflow-hidden">
        <span class="text-2xl p-5 font-semibold block">{{ prod.title }}</span>
    </div>
    </section>
  </div>
</template>
<script>
import abaya from "../assets/abaya.jpg";
import abaya2 from "../assets/abaya2.jpg";
import palazzo from "../assets/palazzo.jpg";
import viel from "../assets/viel.jpg";
import veil2 from "../assets/veil2.jpg";
import hijab2 from "../assets/hijab2.jpg";
export default {
  data() {
    return {
      products: [
        {
          title: "Abaya",
          img: abaya,
        },
        {
          title: "Abaya",
          img: abaya2,
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
          title: "Hijab",
          img: hijab2,
        },
        {
          title: "Veil",
          img: veil2,
        },
      ],
    };
  },
};
</script>
