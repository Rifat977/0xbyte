<template>
  <div class="bg-primary min-h-screen flex flex-col pb-16">
    <Topbar :activeMenu="activeMenu" />
    <Logo />
    <!-- site content -->
    <section class="flex-grow flex flex-col lg:flex-row justify-center items-center lg:pr-36 lg:pl-36">
      <!-- Left Side (text) -->
      <div class="w-full lg:w-1/2 text-white text-center lg:text-left mt-4 lg:mt-0">
        <h3 class="text-xl md:text-3xl lg:text-4xl font-semibold mb-8 mx-4 lg:mx-0">Driving Software Evolution, One Byte at a Time</h3>
        <p class="mb-10 leading-loose text-1xl">
          Discover excellence with 0<span class="text-blue">xByte</span> – your guide to embracing the digital frontier. We specialize in decoding complexities, offering insights, and empowering businesses with transformative solutions. Our passion lies in unraveling innovation, one byte at a time. Join us on a journey of growth and possibilities.
        </p>
        <div class="flex justify-center lg:justify-start space-x-4">
          <button class="outline outline-blue-500 rounded focus:outline-none hover:bg-blue-500 duration-300" style="padding: 10px 20px; border-radius: 8px;">
            Get Started
          </button>
        </div>
      </div>
      <!-- Right Side (image) -->
      <div class="w-full lg:w-1/2 flex items-center lg:justify-end justify-center mt-6 lg:mt-0"> 
        <img src="https://media-public.canva.com/7bK5U/MAEjfy7bK5U/1/s.svg" alt="Image" class="w-96 md:w-108 lg:w-120 h-auto shadow">
      </div>
    </section>
    <section class="py-8 text-center">
      <div class="container mx-auto">
        <div class="grid grid-cols-2 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-8">
          
          <div class="flex flex-col items-center"> 
            <div class="rounded-lg p-2 mt-4 text-center">
              <div class="flex items-center justify-center mb-4">
                <div class="rounded-full bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600 w-20 h-20 flex justify-center items-center">
                  <i class="fa-regular fa-handshake text-white text-2xl"></i>
                </div>
              </div>
              <div class="text-xl text-white font-bold">12+</div>
              <div class="text-xl font-bold text-white">Tech Partners</div>
            </div>
          </div>

          <div class="flex flex-col items-center"> 
            <div class="rounded-lg p-2 mt-4 text-center">
              <div class="flex items-center justify-center mb-4">
                <div class="rounded-full bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600 w-20 h-20 flex justify-center items-center">
                  <i class="fa-regular fa-clock text-white text-2xl"></i>
                </div>
              </div>
              <div class="text-xl text-white font-bold">3+</div>
              <div class="text-xl font-bold text-white">Years of Experience</div>
            </div>
          </div>

          <div class="flex flex-col items-center"> 
            <div class="rounded-lg p-2 mt-4 text-center">
              <div class="flex items-center justify-center mb-4">
                <div class="rounded-full bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600 w-20 h-20 flex justify-center items-center">
                  <i class="fa-solid fa-globe text-white text-2xl"></i>
                </div>
              </div>
              <div class="text-xl text-white font-bold">5+</div>
              <div class="text-xl font-bold text-white">Countries Served</div>
            </div>
          </div>

          <div class="flex flex-col items-center"> 
            <div class="rounded-lg p-2 mt-4 text-center">
              <div class="flex items-center justify-center mb-4">
                <div class="rounded-full bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600 w-20 h-20 flex justify-center items-center">
                  <i class="fa-solid fa-user-tie text-white text-2xl"></i>
                </div>
              </div>
              <div class="text-xl text-white font-bold">10+</div>
              <div class="text-xl font-bold text-white">IT Professionals</div>
            </div>
          </div>

          <div class="flex flex-col items-center"> 
            <div class="rounded-lg p-2 mt-4 text-center">
              <div class="flex items-center justify-center mb-4">
                <div class="rounded-full bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600 w-20 h-20 flex justify-center items-center">
                  <i class="fa-solid fa-check text-white text-2xl"></i>
                </div>
              </div>
              <div class="text-xl text-white font-bold">8+</div>
              <div class="text-xl font-bold text-white">Projects Completed</div>
            </div>
          </div>

  
        </div>
      </div>
    </section>
  </div>
</template>

<style>
* {
  font-family:  system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
</style>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      activeMenu: 'home'
    };
  }
};
</script>
