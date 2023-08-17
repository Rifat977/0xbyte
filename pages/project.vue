<template>
  <div class="bg-primary min-h-screen flex flex-col pb-10">
    <Topbar :activeMenu="activeMenu" />
    <Logo />
    <div class="flex items-center mx-3 md:mx-8 lg:mx-20 mt-8 md:mt-0 lg:mt-4">
      <hr class="flex-grow border-t-1 border-sky-500 ml-4">
      <h3
        class="bg-gradient-to-r from-sky-600 to-indigo-500 text-white text-xl md:text-1xl lg:text-2xl font-bold py-2 px-4 ml-4 rounded-md">
        Our Projects
      </h3>
      <hr class="flex-grow border-t-1 border-blue-500 ml-4">
    </div> 

    <div class="py-8">
      <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="bg-white overflow-hidden shadow-xl sm:rounded-lg">
          <div class="px-4 py-5 sm:p-6">
            <div class="sm:flex sm:items-center">
              <div class="text-center sm:text-left">
                <h3 class="text-lg leading-6 font-medium text-gray-900">
                  Card Title
                </h3>
                <div class="mt-2 text-sm text-gray-500">
                  <p>
                    This is for title
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mt-8 md:mt-6 lg:mt-4 mx-4 md:mx-8 lg:mx-20">
      <!-- Card 1 -->
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
    