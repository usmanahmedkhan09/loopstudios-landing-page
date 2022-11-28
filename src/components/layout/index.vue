<template>
  <HeaderVue />
  <Content />
  <!-- <FooterVue /> -->
</template>
<script lang="ts">
import { defineComponent } from "vue";
import HeaderVue from "./header.vue";
import Content from "./content.vue";
import FooterVue from "./footer.vue";

export default defineComponent({
  components: { HeaderVue, Content, FooterVue },
  setup() {
    return {};
  },
});
</script>
