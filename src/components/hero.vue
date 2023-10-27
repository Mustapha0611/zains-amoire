<template>
  <div
    class="flex md:flex-row flex-col md:h-[90vh] h-auto md:pt-20 pt-5 px-10 md:p-0"
  >
    <section class="flex-1 lg:px-20 md:px-10">
      <div>
        <h2
          class="animate__animated animate__zoomIn animate__faster font-bold py-2 md:py-10 lg:text-6xl text-5xl leading-[1.5] lg:leading-normal" 
        >
          Experience Modest Fashion Like Never Before
        </h2>
        <p class="py-5 animate__animated animate__zoomIn animate__faster">From Timeless Classic to Latest Fashion Pieces</p>
        <div class="py-10 flex md:flex-row flex-col gap-3 animate__animated animate__zoomIn">
          <a
            href=""
            class="text-white px-3 py-3 text-center text-sm lg:px-5 border-2 border-black bg-black md:mr-5 hover:text-black hover:bg-white transition-all"
            >Get Stylishly Modest</a
          >
          <a
            href="#prod"
            class="bg-white px-3 py-3 text-center text-sm lg:px-5 text-black border-2 border-black hover:text-white hover:bg-black transition-all"
            >Check Out Our Products</a
          >
        </div>
      </div>
    </section>
    <section class="flex flex-1 -z-10">
      <div class="flex-1">
        <img
          src="@/assets/img.jpg "
          class="md:w-[85%] w-[90%] md:h-[37vh] h-[23vh] rounded-t-full rounded-e-full grayscale"
          alt=""
        />
        <img
          src="@/assets/bnw.jpg"
          class="mt-5 w-[85%] md:h-[39vh] h-[20vh] object-fit"
          alt=""
        />
      </div>
      <div class="flex-1">
        <img
          src="@/assets/drawer.jpg"
          class="md:w-[90%] w-[95%] md:h-[79vh] h-[45vh] rounded-t-full grayscale"
          alt=""
        />
      </div>
    </section>
  </div>
</template>
