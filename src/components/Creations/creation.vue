<template>
  <div class="creation">
    <div class="creation--header">
      <p class="title">OUR CREATIONS</p>
      <button class="button">SEE ALL</button>
    </div>
    <div class="creation--body">
      <div class="images_wrapper">
        <div class="images" v-for="(image, index) in images" :key="index">
          {{ image.name }}
        </div>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  setup() {
    const images = ref([
      {
        name: "Deep Earth",
        pic: "deep-earth",
      },
      {
        name: "night Arcade",
        pic: "night-arcade",
      },
      {
        name: "the grid",
        pic: "grid",
      },
      {
        name: "from Up Above vr",
        pic: "from-above",
      },
      {
        name: "pocket borealis ",
        pic: "pocket-borealis",
      },
      {
        name: "the curiosity",
        pic: "curiosity",
      },
      {
        name: "make it eyefish",
        pic: "fisheye",
      },
      {
        name: "Soccer team",
        pic: "soccer-team",
      },
    ]);
    return {
      images,
    };
  },
});
</script>
