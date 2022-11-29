<template>
  <footer class="footer">
    <div class="log_wrapper">
      <Logo />
      <ul>
        <li><a href="">About</a></li>
        <li><a href="">Careers</a></li>
        <li><a href="">Events</a></li>
        <li><a href="">Products</a></li>
        <li><a href="">Support</a></li>
      </ul>
    </div>
    <div class="list_wrapper">
      <div class="icons desktop">
        <FacebookIcon />
        <Twitter />
        <Printerest />
        <Instagram />
      </div>
      <p>2021 Loopstudios.All rights reserved</p>
    </div>
  </footer>
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
