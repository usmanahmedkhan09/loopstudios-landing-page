<template>
  <div
    class="sidebar"
    :class="sidebar ? 'open' : ''"
    @click="$emit('closeSidebar')"
  >
    <div class="sidenav"></div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
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
