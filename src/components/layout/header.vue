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
    </div>

    <div class="heading">
      <h1>IMMERSIVE EXPERIENCES THAT DELIVER</h1>
    </div>
  </header>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import LogoIcon from "@/components/icons/logoIcon.vue";

export default defineComponent({
  components: { LogoIcon },
  setup() {
    return {};
  },
});
</script>
