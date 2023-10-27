<template>
    <div class="bg-black text-slate-50 h-[100dvh] flex items-center justify-center z-30">
        <p class="text-4xl border-2 p-4 rounded-xl bounce">Zain_Amoire</p>
    </div>
</template>
<script>
import Button from 'primevue/button';
export default{
    components:{
        Button
    }
}
</script>
<style scoped>
.bounce{
    animation: bouncing 1s linear infinite;
}

@keyframes bouncing {
    0%{
        transform: scale(0.8);
        opacity:0.5;
    }
    50%{
        transform: scale(1);
        opacity:1;
    }
    100%{
        transform: scale(0.8);
        opacity:0.5;
    }
}
</style>