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
            <img class="max-h-8" src="https://assets.stickpng.com/images/5e8ce3cc664eae0004085464.png" alt="Brand 4">
          </div>
          <div class="flex items-center justify-center">
            <img class="max-h-8" src="https://assets.stickpng.com/images/5842a629a6515b1e0ad75afa.png" alt="Brand 5">
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
