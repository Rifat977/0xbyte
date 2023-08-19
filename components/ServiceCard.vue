<template>
    <div class="bg-transparent p-6 rounded shadow-xl">
      <div class="flex items-center justify-center mb-2">
        <img :src="icon" alt="UI/UX Design Icon" class="w-20 h-20">
      </div>
      <h3 class="text-xl font-semibold text-white text-center mt-4">{{title}}</h3>
      <p class="text-gray-200 mt-2">{{ content }}</p>
    </div>
  </template>


<script>
export default {
    props: {
        icon : String,
        title : String,
        content : String
    },
    name: 'ServiceVue'
}
</script>