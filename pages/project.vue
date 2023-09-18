<template>
  <div class="bg-primary min-h-screen flex flex-col pb-10">
    <Topbar :activeMenu="activeMenu" />
    <Logo />
    <div class="pl-6 lg:pr-36 lg:pl-36">
      <nav class="container mx-auto py-6">
        <a href="#" class="text-white font-bold text-xl md:text-xl hover:scale-105">
          Home
        </a>
        <span class="text-white mx-2">/</span>
        <a href="#" class="text-white font-bold text-xl md:text-xl hover:scale-105">
          Our Works
        </a>
      </nav>
    </div>

    <div class="mt-2">
      <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 gap-6 md:grid-cols-2">
          <!-- Card 1 -->
          <div class="overflow-hidden shadow-xl sm:rounded-lg dark:hover:bg-sky-700">
            <div class="px-4 py-5 sm:p-6">
              <div class="sm:flex sm:items-center">
                <div class="text-center sm:text-left">
                  <h3 class="font-medium text-white">
                    Welcome to our project showcase, where innovation meets code. Our journey is marked by a series of captivating website projects that embody creativity, functionality, and user-centric design. With a passion for pushing boundaries, we've brought ideas to life for businesses and individuals alike.
                  </h3>
                </div>
              </div>
            </div>
          </div>
          <!-- Card 2 -->
          <div class="overflow-hidden shadow-xl sm:rounded-lg dark:hover:bg-sky-700">
            <div class="px-4 py-5 sm:p-6">
              <div class="sm:flex sm:items-center">
                <div class="text-center sm:text-left">
                  <h3 class="font-medium text-white">
                    Welcome to our project showcase, where innovation meets code. Our journey is marked by a series of captivating website projects that embody creativity, functionality, and user-centric design. With a passion for pushing boundaries, we've brought ideas to life for businesses and individuals alike.
                  </h3>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>


    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mt-8 md:mt-6 lg:mt-8 mx-4 md:mx-8 lg:mx-20">
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
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
    