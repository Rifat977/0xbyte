<template>
  <div class="bg-primary min-h-screen flex flex-col pb-16">
    <Topbar :activeMenu="activeMenu" />
    <Logo />
    
    <!-- site content -->
    <section class="flex-grow flex flex-col lg:flex-row justify-center items-center lg:pr-36 lg:pl-36">
      <!-- Left Side (text) -->
      <div class="w-full lg:w-1/2 text-white text-center lg:text-left">
        <h3 class="text-xl md:text-3xl lg:text-4xl font-semibold mb-8">Unraveling Excellence with 0<span class="text-blue">xByte's</span></h3>
        <p class="mb-10 leading-loose text-1xl">
          Discover excellence with 0<span class="text-blue">xByte</span> – your guide to embracing the digital frontier. We specialize in decoding complexities, offering insights, and empowering businesses with transformative solutions. Our passion lies in unraveling innovation, one byte at a time. Join us on a journey of growth and possibilities.
        </p>
        <div class="flex justify-center lg:justify-start space-x-4">
          <button class="outline outline-sky-500 rounded focus:outline-none hover:bg-cyan-500 duration-300" style="padding: 10px 20px; border-radius: 8px;">
            Get Started
          </button>
        </div>
      </div>
      <!-- Right Side (image) -->
      <div class="w-full lg:w-1/2 flex items-center lg:justify-end justify-center mt-6 lg:mt-0"> 
        <img src="https://media-public.canva.com/7bK5U/MAEjfy7bK5U/1/s.svg" alt="Image" class="w-96 md:w-108 lg:w-120 h-auto shadow">
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
