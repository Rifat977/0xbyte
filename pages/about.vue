<template>
  <div class="bg-primary min-h-screen flex flex-col pb-10 backdrop-blur font-sans">
        <Topbar :activeMenu="activeMenu" />
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
  