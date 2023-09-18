<template>
  <div class="bg-primary min-h-screen flex flex-col pb-10">
    <Topbar :activeMenu="activeMenu" />
    <Logo />

    <!-- Navigation Links -->
    <div class="lg:pr-36 lg:pl-36 px-4 md:px-0"> <!-- Added px-4 for mobile devices -->
      <nav class="container mx-auto py-6">
        <a href="#" class="text-white font-bold text-xl md:text-xl hover:scale-105">
          Home
        </a>
        <span class="text-white mx-2">/</span>
        <a href="#" class="text-white font-bold text-xl md:text-xl hover:scale-105">
          About Us
        </a>
      </nav>

      <section class="container mx-auto bg-opacity-90 shadow-xl rounded-lg overflow-hidden">
        <div class="grid grid-cols-1 md:grid-cols-2">
          <div class="bg-primary md:p-6 p-4">
            <h2 class="text-3xl font-semibold text-white mb-6">Mission and Vision</h2>
            <p class="text-lg text-gray-200">
              At [Your Company Name], we are passionate about [describe your company's mission or purpose]. Founded in
              [year of establishment], we have been dedicated to [briefly describe your core values, goals, or mission].

              Our team of experts and professionals brings a wealth of experience and knowledge to every project we
              undertake. We are committed to delivering [mention what makes your company unique, such as exceptional
              quality, innovation, or outstanding service] to our clients.

              Over the years, we have [highlight some key achievements or milestones] and have earned a reputation for
              [mention any accolades, industry recognition, or customer testimonials].
            </p>
          </div>
          <div class="">
            <img src="https://media-public.canva.com/2D-hU/MAEbhJ2D-hU/1/s2-1.svg" alt="Mission and Vision Image"
              class="rounded-lg mx-auto h-full p-6">
          </div>
        </div>
      </section>

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
