<template>
  <div class="creation">
    <div class="creation--header">
      <p class="title">OUR CREATIONS</p>
      <button class="button desktop">SEE ALL</button>
    </div>
    <div class="creation--body">
      <div class="images_wrapper">
        <div
          class="image"
          v-for="(image, index) in images"
          :key="index"
          :style="{ backgroundImage: `url(${getImageUrl(image.pic)})` }"
        >
          <h1>{{ image.name }}</h1>
        </div>
      </div>
    </div>
    <div class="button_wrapper">
      <button class="button mobile">SEE ALL</button>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";
import { useMediaQuery } from "@vueuse/core";

export default defineComponent({
  setup() {
    const isMediumScreen = ref(useMediaQuery("(max-width: 768px)"));
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
        name: "Soccer team",
        pic: "soccer-team",
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
    ]);

    const getImageUrl = (name: any) => {
      let pic = new URL(
        `../../assets/images/${
          isMediumScreen.value ? "mobile" : "desktop"
        }/image-${name}.jpg`,
        import.meta.url
      ).href;
      return pic;
    };
    return {
      images,
      isMediumScreen,
      getImageUrl,
    };
  },
});
</script>
