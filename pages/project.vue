<template>
  <div class="bg-primary min-h-screen flex flex-col pb-10">
    <Topbar :activeMenu="activeMenu" />
    <Logo />
    <div class="flex items-center mx-3 md:mx-8 lg:mx-20 mt-8 md:mt-0 lg:mt-4">
      <hr class="flex-grow border-t-1 border-sky-500 ml-4">
    <h3 class="bg-gradient-to-r from-sky-600 to-indigo-500 text-white text-xl md:text-1xl lg:text-2xl font-bold py-2 px-4 ml-4 rounded-md">
         Our Projects 
    </h3>
    <hr class="flex-grow border-t-1 border-blue-500 ml-4">
</div>



<!-- <hr class="border-t-2 border-white my-2 mx-4 md:mx-8 lg:mx-20"> -->

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mt-8 md:mt-6 lg:mt-8 mx-4 md:mx-8 lg:mx-20">
      <!-- Card 1 -->
      <Card/>
      <Card/>
      <Card/>
      <Card/>
      <Card/>
      <Card/>


    </div>
  </div>
</template>

  
    
<script>
import Swiper from 'swiper/swiper-bundle.min';
import 'swiper/swiper-bundle.min.css';

export default {
  name: 'ProjectPage',
  data() {
    return {
      activeMenu: 'project'
    };
  },
  mounted() {
    new Swiper(this.$refs.swiper, {
      pagination: {
        el: '.swiper-pagination',
        clickable: true,
      },
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
    });
  },
};
</script>
    