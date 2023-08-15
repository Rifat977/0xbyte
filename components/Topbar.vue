<template>
  <div class="sticky bottom-0 left-0 w-full bg-primary flex justify-between py-2 pl-4 pr-4 shadow-md">
    <nuxt-link
      v-for="(menuItem, index) in menuItems"
      :key="index"
      :class="{ 'active-menu': activeMenu === menuItem.id }"
      class="focus:outline-none text-center"
      @click="toggleMenu(menuItem.id)"
      :to="menuItem.id === 'home' ? '/' : menuItem.id"
    >
      <div
        :class="{ 'bg-blue': activeMenu === menuItem.id, 'bg-transparent': activeMenu !== menuItem.id }"
        class="w-12 h-12 flex flex-col items-center justify-center rounded-full transition duration-300"
      >
        <i
          v-if="menuItem.icon !== '0xByte'"
          :class="[
            menuItem.icon,
            activeMenu === menuItem.id ? 'text-white' : 'text-white'
          ]"
        ></i>
        <div v-else class="text-white text-xl lg:text-2xl font-bold">0<span class="text-blue">x</span>Byte</div>
        <!-- <div v-if="menuItem.icon !== '0xByte'" class="text-xs mt-1 text-blue">{{ menuItem.name }}</div> -->
      </div>
    </nuxt-link>
  </div>
</template>
  
  <style>
  .bg-primary {
    background: linear-gradient(135deg, #1d3a70, #134864, #25333a, #1e4067, #3f5d5f);
    background-size: 400% 400%;
    /* animation: gradientAnimation 15s ease infinite; */
  }

@keyframes gradientAnimation {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
  
  .text-primary {
    color: #0f172a;
  }

  .text-blue {
    color:#45c0ec;
  }

  .bg-blue{
    background-color: #45c0ec;
  }
  
  .active-menu {
    color: #ffffff;
    font-weight: bold;
  }
  .active-menu {
    color: #ffffff;
    font-weight: bold;
    }
    .btn-primary {
    background-color: #45c0ec;
    color: #fff;
    padding: 10px 20px;
    border-radius: 8px;
    text-decoration: none;
    transition: background-color 0.3s;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
    }

    .btn-primary:hover {
    background-color: #3490dc;
    }
  </style>
  
<script>
export default {
  props: {
    activeMenu: String,
  },
  data() {
    return {
      menuItems: [
        { id: 'home', icon: 'fas fa-home', name: 'Home' },
        { id: 'about', icon: 'fas fa-info-circle', name: 'About' },
        { id: '0xByte', icon: '0xByte', name: '0xByte' },
        { id: 'services', icon: 'fas fa-cogs', name: 'Services' },
        { id: 'contact', icon: 'fas fa-envelope', name: 'Contact' },
      ],
    };
  },
  methods: {
    toggleMenu(menu) {
      this.activeMenu = this.activeMenu === menu ? null : menu;
    },
  },
  name: 'Topbar',
};
</script>
  