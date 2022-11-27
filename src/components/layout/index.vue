<template>
  <HeaderVue />
  <Content />
</template>
<script lang="ts">
import { defineComponent } from "vue";
import HeaderVue from "./header.vue";
import Content from "./content.vue";

export default defineComponent({
  components: { HeaderVue, Content },
  setup() {
    return {};
  },
});
</script>
