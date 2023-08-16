<template>
    <div class="block max-w-sm border border-gray-200 rounded-lg shadow hover:bg-gray-100 dark:border-gray-700 dark:hover:bg-gray-700 mb-10" style="background: linear-gradient(135deg, #011d44, #214378, #122652);">
          <img src="~/assets/project.jpg" alt="Project Image" class="w-full object-cover mb-4 rounded-md">
          <div class="px-6 py-4">
              <h4 class="text-xl font-semibold text-white mb-2">Project Title</h4>
              <p class="text-white mb-4">Short description of the project.</p>
              <button class="bg-gradient-to-r from-sky-600 to-blue-500 hover:to-blue-600 text-white py-2 px-4 rounded-md shadow-md hover:shadow-lg focus:outline-none focus:ring focus:ring-blue-300 transition duration-300 ease-in-out">
                Learn More
              </button>
          </div>
          <div class="px-6 pt-4 pb-4">
              <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#nuxt</span>
              <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#tailwind css</span>
              <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#bootstrap</span>
          </div>
      </div>
</template>

<script>
    export default{
        name: "Card"
    }
</script>