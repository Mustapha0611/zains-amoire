<template>
    <div class="bg-black text-slate-50 h-[100dvh] flex items-center justify-center z-30">
        <p class=" p-5 w-44 h-[170px] bounce rounded-full"><img src="@/assets/logo.png" alt=""></p>
    </div>
</template>
<script>
export default{
    components:{
   
    }
}
</script>
<style scoped>


@keyframes bouncing {
    0%{
        transform: scale(0.8);
        opacity:0.8;
    }
    50%{
        transform: scale(1);
        opacity:1;
    }
    100%{
        transform: scale(0.8);
        opacity:0.8;
    }
}
</style>