<template>
  <main class="content">
    <div class="section--one">
      <div class="image_wrapper">
        <img src="../../assets/images/desktop/image-interactive.jpg" alt="" />
      </div>
      <div class="card">
        <h1>THE LEADER IN INTERACTIVE VR</h1>
        <p>
          Founded in 2011, Loopstudios has been producing world-class virtual
          reality projects fro some of the best companies around the globe. Our
          award-wining creations have transfromed bussiness through digital
          experience that bind to their brand.
        </p>
      </div>
    </div>
    <CreationVue />
    <FooterVue />
  </main>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import CreationVue from "../Creations/creation.vue";
import FooterVue from "./footer.vue";

export default defineComponent({
  components: { CreationVue, FooterVue },
  setup() {
    return {};
  },
});
</script>
