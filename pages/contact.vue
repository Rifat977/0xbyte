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
          Contact
        </a>
      </nav>
    </div>

    <div class="lg:pr-36 lg:pl-36 mb-10">
      <div class="max-w-2xl mx-auto px-4 sm:px-6 lg:max-w-7xl lg:px-8">
        <div class="bg-transparent overflow-hidden shadow-xl sm:rounded-lg p-6 text-center">
          <h1 class="text-4xl font-semibold text-white mb-4">
            Let's Connect and Create Something Amazing
          </h1>
          <p class="text-lg text-gray-200">
            Ready to start a project with us? Let's talk!
          </p>
        </div>

        <div class="overflow-hidden shadow-xl sm:rounded-lg mt-6 p-6">
          <dl class="grid grid-cols-1 gap-x-4 gap-y-6 sm:grid-cols-3">
            <div class="sm:col-span-1">
              <dt class="text-sm font-medium text-white">
                Email
              </dt>
              <dd class="mt-1 text-sm text-gray-400">
                info@0xbyte.com
              </dd>
            </div>
            <div class="sm:col-span-1">
              <dt class="text-sm font-medium text-white">
                Phone Number
              </dt>
              <dd class="mt-1 text-sm text-gray-400">
                +88 017 3650 6590
              </dd>
            </div>
            <div class="sm:col-span-1">
              <dt class="text-sm font-medium text-white">
                Phone Number
              </dt>
              <dd class="mt-1 text-sm text-gray-400">
                +88 017 3650 6590
              </dd>
            </div>
            <div class="sm:col-span-3">
              <dt class="text-sm font-medium text-white">
                Name
              </dt>
              <input type="text" class="mt-1 p-3 w-full border rounded-md focus:ring-indigo-500 focus:border-indigo-500"
                placeholder="Your Name" />
            </div>
            <div class="sm:col-span-3">
              <dt class="text-sm font-medium text-white">
                Email
              </dt>
              <input type="email" class="mt-1 p-3 w-full border rounded-md focus:ring-indigo-500 focus:border-indigo-500"
                placeholder="Your Email" />
            </div>
            <div class="sm:col-span-3">
              <dt class="text-sm font-medium text-white">
                Phone Number
              </dt>
              <input type="tel" class="mt-1 p-3 w-full border rounded-md focus:ring-indigo-500 focus:border-indigo-500"
                placeholder="Your Phone Number" />
            </div>
            <div class="sm:col-span-3">
              <dt class="text-sm font-medium text-white">
                Message
              </dt>
              <textarea rows="4" class="mt-1 p-3 w-full border rounded-md focus:ring-indigo-500 focus:border-indigo-500"
                placeholder="Your Message"></textarea>
            </div>
          </dl>
        </div>
        <div class="bg-transparent overflow-hidden sm:rounded-lg mt-6 p-6">
          <button
            class="inline-flex items-center justify-center w-full px-6 py-3 border border-transparent rounded-md shadow-sm text-base font-medium text-white bg-sky-700 hover:bg-sky-800 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500 transition-transform transform hover:scale-105">
            Submit
          </button>
        </div>

      </div>
    </div>

  </div>
</template>
  
    
<script>
export default {
  name: 'ContactPage',
  data() {
    return {
      activeMenu: 'contact'
    };
  }
};
</script>
    