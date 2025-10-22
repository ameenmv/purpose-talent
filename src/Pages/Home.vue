<template>
  <div class="home">
    <Landing />
    <Section2 />
  </div>
</template>

<script>
import gsap from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";
gsap.registerPlugin(ScrollTrigger);

import Landing from "../components/Landing.vue";
import Section2 from "../components/section2.vue";

export default {
  name: "Home",
  components: {
    Landing,
    Section2,
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
