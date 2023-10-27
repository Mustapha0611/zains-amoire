<template>
  <header
    class="flex w-full h-[10vh] shadow-md justify-evenly items-center md:pl-10 pl-5 pr-12 top-0 left-0"
  >
    <span
      class="md:hidden absolute top-5 right-5 text-2xl text-slate-100 cursor-pointer"
      @click="toggleMenu"
    >
      <img src="@/assets/menu.png" alt="" />
    </span>
    <div class="logo flex-1">
      <span class="px-1 md:text-2xl text-xl"
        >
        <img src="@/assets/logo.png" class="md:w-20 w-16 h-10 " alt="">
        </span
      >
    </div>

    <nav class="flex-2">
      <ul
        class="flex md:justify-start justify-center md:items-start transition-all items-center text-slate-50 md:text-slate-800 font-semibold md:flex-row flex-col md:relative absolute w-full h-[100vh] md:h-12 -left-[100%] md:transform-none top-0 md:left-0 bg-black md:bg-white"
        :class="{ show: showMenu }"
      >
        <span
          class="md:hidden absolute top-5 right-5 w-5 text-lime-100 cursor-pointer"
          @click="toggleMenu"
          >
          <img src="../assets/close.png" alt="" class="w-full h-full">
          </span
        >
        <li class="py-2 px-4">
          <a
            href=""
            class="pb-4 md:hover:text-slate-800 hover:border-b-2 hover:border-b-gray-400 md:hover:border-b-slate-900 hover:text-gray-300"
            @click="toggleMenu"
            >Home</a
          >
        </li>
        <li class="py-2 px-4">
          <a
            href="#abt"
            class="pb-4 md:hover:text-slate-800 hover:border-b-2 hover:border-b-gray-400 md:hover:border-b-slate-900 hover:text-gray-300"
            @click="toggleMenu"
            >About</a
          >
        </li>
        <li class="py-2 px-4">
          <a
            href="#prod"
            class="pb-4 md:hover:text-slate-800 hover:border-b-2 hover:border-b-gray-400 md:hover:border-b-slate-900 hover:text-gray-300"
            @click="toggleMenu"
            >Products</a
          >
        </li>
        <li class="py-2 px-4">
          <a
            href="#faq"
            class="pb-4 md:hover:text-slate-800 hover:border-b-2 hover:border-b-gray-400 md:hover:border-b-slate-900 hover:text-gray-300"
            @click="toggleMenu"
            >FAQs</a
          >
        </li>
        <div
          class="flex justify-between md:relative absolute bottom-12 right-[35%] md:right-0 md:top-0 text-2xl text-gray-50 md:text-slate-950 cursor-pointer"
        >
          <a
            href="#contact"
            class="px-10 py-2 text-sm border-2 border-slate-700 rounded-md"
            @click="toggleMenu"
          >
            Contact
          </a>
        </div>
      </ul>
    </nav>
  </header>
</template>
<script>
import Button from "primevue/button";
export default {
  components: {
    Button,
  },
  data() {
    return {
      showMenu: false,
    };
  },
  methods: {
    toggleMenu() {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>
<style>
a:focus {
  color: black;
  border-bottom: 3px solid rgb(2, 2, 2);
}
.show {
  transform: translateX(100%);
  transition: 0.4s all;
}
@media screen and (min-width: 768px) {
  .show {
    transform: translateX(0%);
    transition: 0.1s all;
  }
}
</style>
