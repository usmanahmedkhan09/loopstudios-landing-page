<template>
  <div
    class="sidebar"
    :class="sidebar ? 'open' : ''"
    @click="$emit('closeSidebar')"
  >
    <div class="sidenav">
      <div class="cross_icon">
        <CloseIconVue />
      </div>
      <ul>
        <li><a href="">About</a></li>
        <li><a href="">Careers</a></li>
        <li><a href="">Events</a></li>
        <li><a href="">Products</a></li>
        <li><a href="">Support</a></li>
      </ul>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import CloseIconVue from "../icons/CloseIcon.vue";

export default defineComponent({
  components: { CloseIconVue },
  props: {
    sidebar: {
      type: Boolean,
      required: true,
    },
  },
  setup() {
    return {};
  },
});
</script>
