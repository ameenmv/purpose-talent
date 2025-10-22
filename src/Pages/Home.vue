<template>
  <div class="home">
    

      <Landing />

  </div>
</template>

<script>
import gsap from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";
gsap.registerPlugin(ScrollTrigger);

import Landing from "../components/Landing.vue";

export default {
  name: "Home",
  components: {

    Landing,
  },
  mounted() {
    // gsap.to(".section1", {
    //   scrollTrigger: {},
    // });
  },
};
</script>

<style lang="scss" scoped>
.home {
  background: var(--bg-color);
}
</style>
