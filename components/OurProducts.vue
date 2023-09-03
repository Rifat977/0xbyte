<template>
    <div class="bg-transparent rounded-lg shadow-xl p-6 relative flex">
        <div class="mr-4">
            <i class="fa-solid fa-shop text-blue-500 text-3xl"></i>
        </div>
        <div>
            <h3 class="text-lg font-semibold text-white mb-2">{{ name }}</h3>
            <p class="text-gray-300">{{ description }}</p>
        </div>
        <span
            class="bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600 text-white py-1 px-2 rounded-full text-sm absolute top-2 right-2">{{ category }}</span>
    </div>
</template>
  
<script>
export default {
    props: {
        name: String,
        description: String,
        category: String
    },
};
</script>
  