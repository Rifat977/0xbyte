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
          Our Services
        </a>
      </nav>
    </div>

    <section class="bg-transparent py-8 mt-8 lg:pr-36 lg:pl-36">
      <div class="container px-4 lg:px-0">
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <ServiceCard :icon="'https://media-public.canva.com/CNMy8/MAELw7CNMy8/1/s.svg'" :title="'UI/UX Design'"
            :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'" />
          <ServiceCard :icon="'https://media-public.canva.com/exODI/MAFf8PexODI/1/s-1.svg'"
            :title="'Web Application Development'"
            :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'" />
          <ServiceCard :icon="'https://media-public.canva.com/BlRJw/MAE-heBlRJw/1/tl.png'"
            :title="'Mobile Apps Development'"
            :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'" />
          <ServiceCard :icon="'https://media-public.canva.com/b1-LI/MAFme8b1-LI/1/s.svg'" :title="'Application Security'"
            :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'" />
          <ServiceCard :icon="'https://media-public.canva.com/ubcts/MAFV66ubcts/1/s-1.svg'" :title="'DevOps & Cloud'"
            :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'" />
          <ServiceCard :icon="'https://media-public.canva.com/09s6s/MAFgq009s6s/1/s-1.svg'" :title="'AI & ML'"
            :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'" />
        </div>
      </div>
    </section>

  </div>
</template>
  
    
<script>
export default {
  name: 'ServicePage',
  data() {
    return {
      activeMenu: 'services'
    };
  }
};
</script>
    