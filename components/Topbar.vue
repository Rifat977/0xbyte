<template>
  <div class="sticky bottom-0 left-0 w-full bg-primary flex justify-between py-2 pl-4 pr-4 shadow" style="position: fixed;">
    <nuxt-link
      v-for="(menuItem, index) in menuItems"
      :key="index"
      :class="{ 'active-menu': activeMenu === menuItem.id }"
      class="focus:outline-none text-center"
      @click="toggleMenu(menuItem.id)"
      :to="menuItem.id === 'home' ? '/' : menuItem.id"
    >
      <div
        :class="{ 'bg-gradient-to-r from-sky-600 to-blue-500 hover:to-sky-600': activeMenu === menuItem.id, 'bg-slate-900': activeMenu !== menuItem.id }"
        class="w-10 h-10 flex flex-col items-center justify-center rounded-full transition duration-300"
      >
        <i
          :class="[
            menuItem.icon,
            activeMenu === menuItem.id ? 'text-white' : 'text-white'
          ]"
        ></i>
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
        { id: 'about', icon: 'fas fa-users', name: 'About' },
        { id: 'project', icon: 'fa-solid fa-code', name: 'Project' },
        { id: 'home', icon: 'fas fa-home', name: 'Home' },
        { id: 'services', icon: 'fas fa-toolbox', name: 'Services' },
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
  