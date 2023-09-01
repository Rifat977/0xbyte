<template>
  <div class="bg-primary min-h-screen flex flex-col pb-16">
    <Topbar :activeMenu="activeMenu" />
    <Logo />
    <!-- site content -->
    <section class="flex-grow flex flex-col lg:flex-row justify-center items-center lg:pr-36 lg:pl-36">
      <!-- Left Side (text) -->
      <div class="w-full lg:w-1/2 text-white text-center lg:text-left mt-4 lg:mt-0">
        <h3 class="text-xl md:text-3xl lg:text-4xl font-semibold mb-8 mx-4 lg:mx-0">Driving Software Evolution, Infinity Byte at a Time</h3>
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

    <section class="py-8 mt-8 lg:pr-36 lg:pl-36">
      <div class="container px-4 lg:px-0">
        <div class="justify-center items-center">
          <h2 class="text-4xl font-bold mb-10 text-center text-white"><i class="fa-solid fa-minus"></i> 0xByte's Service Excellence</h2>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <ServiceCard :icon="'https://media-public.canva.com/CNMy8/MAELw7CNMy8/1/s.svg'" :title="'UI/UX Design'" :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'"/>
          <ServiceCard :icon="'https://media-public.canva.com/exODI/MAFf8PexODI/1/s-1.svg'" :title="'Web Application Development'" :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'"/>
          <ServiceCard :icon="'https://media-public.canva.com/BlRJw/MAE-heBlRJw/1/tl.png'" :title="'Mobile Apps Development'" :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'"/>
          <ServiceCard :icon="'https://media-public.canva.com/b1-LI/MAFme8b1-LI/1/s.svg'" :title="'Application Security'" :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'"/>
          <ServiceCard :icon="'https://media-public.canva.com/ubcts/MAFV66ubcts/1/s-1.svg'" :title="'DevOps & Cloud'" :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'"/>
          <ServiceCard :icon="'https://media-public.canva.com/09s6s/MAFgq009s6s/1/s-1.svg'" :title="'AI & ML'" :content="'Our UI/UX design service enhances user experiences through intuitive interfaces, seamless interactions, and captivating visuals, fostering meaningful connections between users and digital solutions.'"/>
        </div>
      </div>
    </section>

    <div class="py-8 mt-8 lg:px-36">
      <div class="container px-4 lg:px-0">
        <div class="justify-center items-center">
          <h2 class="text-4xl font-bold mb-12 text-center text-white"><i class="fa-solid fa-minus"></i> 0xByte's Works</h2>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-1 gap-8">

          <div class="flex flex-col md:flex-row bg-transparent rounded-lg shadow-lg">
            <div class="md:w-1/2">
              <img src="https://cdn-developer-wp.arc.dev/wp-content/uploads/2021/12/Do-I-Need-a-Software-Engineering-Degree.jpg" alt="Product 1" class="w-full h-auto md:h-full rounded-lg">
            </div>
            <div class="md:w-1/2 p-4 md:p-0 md:pl-4">
              <h2 class="text-2xl font-bold mb-2 text-white">0xbyte's Point of Sale</h2>
              <p class="leading-loose text-white">
                POS (Point of Sale) system is a innovative software solution that empowers businesses in the retail industry to streamline their operations and enhance customer experiences. 0xbyte's POS system optimizes the entire sales process. From tracking sales in real-time to managing customer loyalty programs. 
                POS (Point of Sale) system is a innovative software solution that empowers businesses in the retail industry to streamline their operations and enhance customer experiences. 0xbyte's POS system optimizes the entire sales process. From tracking sales in real-time to managing customer loyalty programs.
              </p>
              <button class="mt-6 mb-4 bg-blue-500 text-white px-4 py-2 rounded-md hover:bg-blue-600">Order Now</button>
            </div>
          </div>

          <div class="flex flex-col md:flex-row bg-transparent rounded-lg shadow-lg">
            <div class="md:w-1/2">
              <img src="https://www.productplan.com/uploads/2019/12/software-development-lifecycle-1.png" alt="Product 1" class="w-full h-auto md:h-full rounded-lg">
            </div>
            <div class="md:w-1/2 p-4 md:p-0 md:pl-4">
              <h2 class="text-2xl font-bold mb-2 text-white">0xbyte's CRM</h2>
              <p class="leading-loose text-white">
                POS (Point of Sale) system is a innovative software solution that empowers businesses in the retail industry to streamline their operations and enhance customer experiences. 0xbyte's POS system optimizes the entire sales process. From tracking sales in real-time to managing customer loyalty programs. 
                0xbyte's POS system optimizes the entire sales process. From tracking sales in real-time to managing customer loyalty programs.
              </p>
              <button class="mt-6 mb-4 bg-blue-500 text-white px-4 py-2 rounded-md hover:bg-blue-600">Order Now</button>
            </div>
          </div>

        </div>
      </div>
    </div>

    
    <div class="py-8 mt-8 lg:px-36">
      <div class="container px-4 lg:px-0">
        <div class="text-center mb-12">
          <h2 class="text-4xl font-bold text-white">
            <i class="fas fa-minus text-white"></i> Exclusive Products
          </h2>
        </div>
        
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- Card 1 -->
          <div class="bg-transparent rounded-lg shadow-xl p-6 relative flex">
            <div class="mr-4">
              <i class="fa-solid fa-shop text-blue-500 text-3xl"></i>
            </div>
            <div>
              <h3 class="text-lg font-semibold text-white mb-2">Shop MS</h3>
              <p class="text-gray-300">The all-in-all ERP Solution that can integrate every part of any Enterprise-level organization into one single platform.</p>
            </div>
            <span class="bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600 text-white py-1 px-2 rounded-full text-sm absolute top-2 right-2">Jewelry</span>
          </div>
          
          <!-- Card 2 -->
          <div class="bg-transparent rounded-lg shadow-xl p-6 relative flex">
            <div class="mr-4">
              <i class="fa-solid fa-truck-fast text-blue-500 text-3xl"></i>
            </div>
            <div>
              <h3 class="text-lg font-semibold text-white mb-2">Courier DS</h3>
              <p class="text-gray-300">The all-in-all ERP Solution that can integrate every part of any Enterprise-level organization into one single platform.</p>
            </div>
            <span class="bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600 text-white py-1 px-2 rounded-full text-sm absolute top-2 right-2">Electronics</span>
          </div>
          
          <!-- Card 3 -->
          <div class="bg-transparent rounded-lg shadow-xl p-6 relative flex">
            <div class="mr-4">
              <i class="fa-solid fa-money-bill text-blue-500 text-3xl"></i>
            </div>
            <div>
              <h3 class="text-lg font-semibold text-white mb-2">0xbyte CRM</h3>
              <p class="text-gray-300">The all-in-all ERP Solution that can integrate every part of any Enterprise-level organization into one single platform.</p>
            </div>
            <span class="bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600 text-white py-1 px-2 rounded-full text-sm absolute top-2 right-2">Furniture</span>
          </div>
        </div>
      </div>
    </div>

    <div class="py-8 mt-8 lg:px-36">
      <div class="container px-4 lg:px-0">
        <div class="text-center mb-12">
          <h2 class="text-4xl font-bold text-white">
            <i class="fas fa-minus text-white"></i> Brands That Trust Us
          </h2>
        </div>
        
        <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-8">
          <div class="flex items-center justify-center">
            <img class="max-h-8" src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c9/Google_logo_%282013-2015%29.svg/1024px-Google_logo_%282013-2015%29.svg.png" alt="Brand 1">
          </div>
          <div class="flex items-center justify-center">
            <img class="max-h-8" src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ab/Meta-Logo.png/2560px-Meta-Logo.png" alt="Brand 2">
          </div>
          <div class="flex items-center justify-center">
            <img class="max-h-8" src="https://www.edigitalagency.com.au/wp-content/uploads/Spotify_Logo-png-RGB-Green.png" alt="Brand 3">
          </div>
          <div class="flex items-center justify-center">
            <img class="max-h-8" src="data:image/png;base64,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" alt="Brand 4">
          </div>
          <div class="flex items-center justify-center">
            <img class="max-h-8" src="https://gpm.nasa.gov/sites/default/files/document_files/NASA-Logo-Large.png" alt="Brand 5">
          </div>
          <div class="flex items-center justify-center">
            <img class="max-h-8" src="https://assets.stickpng.com/images/5842a770a6515b1e0ad75afe.png" alt="Brand 6">
          </div>
          <div class="flex items-center justify-center">
            <img class="max-h-8" src="https://www.edigitalagency.com.au/wp-content/uploads/airbnb-logo-png-transparent-background.png" alt="Brand 7">
          </div>
          <div class="flex items-center justify-center">
            <img class="max-h-8" src="https://yespartners.com/wp-content/uploads/2017/08/ibm-logo-png-transparent-background.png" alt="Brand 8">
          </div>
        </div>
      </div>
    </div>








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
