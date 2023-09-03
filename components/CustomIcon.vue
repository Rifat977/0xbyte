<template>
    <div class="flex items-center space-x-2 text-gray-400">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        class="h-5 w-5"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M12 6v6m0 0v6m0-6h6m-6 0H6"
        />
      </svg>
      <span class="text-sm font-medium">{{ text }}</span>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      text: String,
    },
  };
  </script>
  