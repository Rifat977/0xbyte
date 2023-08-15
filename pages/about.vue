<template>
  <div class="bg-primary min-h-screen flex flex-col pb-10">
        <Topbar :activeMenu="activeMenu" />
        <Logo />
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
  