<template>
<div class="bg-gray-100 mt-10">
    <h2 class="text-center font-semibold md:text-6xl text-4xl mt-10 mb-5 py-5">Reviews</h2>
      <Carousel :value="reviews" :numVisible="3" :numScroll="1" :responsiveOptions="responsiveOptions" :autoplayInterval="5000">
    <template #item="slotProps">
        <div class="border-2 m-2  py-16 px-3 rounded-md shadow-lg min-h-[200px] md:min-h-[210px] mx-5">
            <div class="mb-3">
                "{{ slotProps.data.comment }}"
            </div>
            <div>
            
                <div class="mt-5">
                    <Avatar  :label="slotProps.data.label" class="mr-2" size="small" shape="circle" />{{ slotProps.data.name }}
                </div>
            </div>
        </div>
    </template>
</Carousel>
</div>
</template>
<script>
import Carousel from 'primevue/carousel';
import Avatar from 'primevue/avatar';
export default {
components:{
    Carousel,
    Avatar
},
data() {
    return {
      reviews: [
        {
          name: "Sarah A.",
          rating: 5,
          label:'S',
          comment:
            "Zain Amoire offers the most beautiful and comfortable hijabs I've ever worn. The quality is outstanding, and their customer service is exceptional. Highly recommended!",
        },
        {
          name: "Ahmed B.",
          rating: 4.5,
          label:'A',
          comment:
            "I recently purchased a veil from Zain Amoire, and I'm impressed with the elegant design and soft fabric. The attention to detail is evident. Will definitely shop here again.",
        },
        {
          name: "Fatima K.",
          rating: 5,
          label:'F',
          comment:
            "Zain Amoire's palazzo pants are a game-changer! They fit perfectly and are so stylish. I love how they combine modesty with fashion. The colors are vibrant, and the material is top-notch.",
        },
        {
          name: "Omar S.",
          rating: 4,
          label:'O',
          comment:
            "Great variety of hijabs at Zain Amoire. The different styles and patterns make it easy to find something for every occasion. Quality is good, and the prices are reasonable. Satisfied with my purchase!",
        },
        {
          name: "Layla H.",
          rating: 4.5,
          label:'L',
          comment:
            "Zain Amoire exceeded my expectations. The veils are elegant, and the customer service team was helpful in assisting me to choose the right one. Quick delivery and excellent packaging. Will shop here again for sure.",
        },
        {
          name: "Aisha N.",
          rating: 5,
          label:'A',
          comment:
            "Zain Amoire offers a fantastic selection of hijabs and palazzo pants. The quality is unmatched, and the designs are unique. I'm always complimented when I wear their products. Fast shipping too!",
        },
        {
          name: "Yusuf M.",
          rating: 4,
          label:'Y',
          comment:
            "I bought a veil from Zain Amoire and was pleasantly surprised by the elegant packaging. The veil itself is beautiful, and the fabric feels luxurious. I appreciate the attention to detail. Great job!",
        },
        {
          name: "Nadia R.",
          rating: 5,
          label:'N',
          comment:
            "Zain Amoire understands modest fashion perfectly. Their palazzo pants are not only stylish but also very comfortable. The hijabs are breathable and versatile. I'm a loyal customer now!",
        },
        {
          name: "Khalid A.",
          rating: 4.5,
          label:'K',
          comment:
            "I've been searching for high-quality veils, and Zain Amoire delivered. The veils are lightweight, yet they provide excellent coverage. The colors are vibrant, and they wash well too. Very satisfied with my purchase.",
        },
        {
          name: "Amira F.",
          rating: 5,
          label:'A',   
          comment:
            "Zain Amoire has become my go-to store for modest fashion. The variety, quality, and affordability are unbeatable. Plus, their customer service team is friendly and responsive. Highly recommended for anyone looking for stylish modest wear!",
        },
      ],
     responsiveOptions: [
                {
                    breakpoint: '1199px',
                    numVisible: 1,
                    numScroll: 1
                },
                {
                    breakpoint: '1198px',
                    numVisible: 2,
                    numScroll: 1
                },
                {
                    breakpoint: '767px',
                    numVisible: 1,
                    numScroll: 1
                }
            ]
    };
  },
};
</script>
