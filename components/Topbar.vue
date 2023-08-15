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
  