<template>
  <div class="footer">
    <div class="log_wrapper">
      <Logo />
      <div class="icons">
        <FacebookIcon />
        <Twitter />
        <Printerest />
        <Instagram />
      </div>
    </div>
    <div class="list_wrapper">
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
import Logo from "@/components/icons/logoIcon.vue";
import FacebookIcon from "@/components/icons/facebook.vue";
import Printerest from "@/components/icons/pinterest.vue";
import Instagram from "@/components/icons/instagram.vue";
import Twitter from "@/components/icons/twitter.vue";

export default defineComponent({
  components: { Logo, FacebookIcon, Printerest, Instagram, Twitter },
  setup() {
    return {};
  },
});
</script>
