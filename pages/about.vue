<template>
  <div class="bg-primary min-h-screen flex flex-col pb-10">
        <Topbar :activeMenu="activeMenu" />
        <Logo />
        <div class="pl-6 lg:pr-36 lg:pl-36">
          <div class="container mx-auto flex items-center space-x-4">
            <a href="#" class="text-white font-bold text-xl md:text-xl flex items-center space-x-2 transition-transform transform hover:scale-105">
              Home
            </a>
            <div class="h-8 w-px bg-white"></div>
            <a href="#" class="text-white font-bold text-xl md:text-xl flex items-center space-x-2 transition-transform transform hover:scale-105">
              About Us
            </a>
          </div>
        </div>




    </div>
</template>

  
  <script>
  export default {
    name: 'AboutPage',
    data() {
    return {
      activeMenu: 'about'
    };
  }
  };
  </script>
  