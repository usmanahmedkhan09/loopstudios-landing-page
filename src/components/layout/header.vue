<template>
  <header class="header">
    <div class="navbar">
      <div class="logo">
        <LogoIcon />
      </div>
      <nav>
        <ul>
          <li>About</li>
          <li>Careers</li>
          <li>Events</li>
          <li>Products</li>
          <li>Support</li>
        </ul>
      </nav>
      <MenuVue @click="sidebar = true" class="menu_icon" />
    </div>
    <div class="heading">
      <h1>IMMERSIVE EXPERIENCES THAT DELIVER</h1>
    </div>
    <SidebarVue
      :sidebar="sidebar"
      v-if="sidebar"
      @closeSidebar="sidebar = false"
    />
  </header>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";
import LogoIcon from "@/components/icons/logoIcon.vue";
import MenuVue from "../icons/menu.vue";
import SidebarVue from "./sidebar.vue";

export default defineComponent({
  components: { LogoIcon, MenuVue, SidebarVue },
  setup() {
    const sidebar = ref(false);
    return {
      sidebar,
    };
  },
});
</script>
