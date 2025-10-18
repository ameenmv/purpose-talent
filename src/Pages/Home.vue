<template>
  <div class="home">
    <div class="h-[100vh]">
      <Navbar />
      <Landing />
    </div>
  </div>
</template>

<script>
import gsap from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";
gsap.registerPlugin(ScrollTrigger);
import Navbar from "../components/Navbar.vue";
import Landing from "../components/Landing.vue";

export default {
  name: "Home",
  components: {
    Navbar,
    Landing,
  },
  mounted() {
    gsap.to(".section1", {
      scrollTrigger: {},
    });
  },
};
</script>

<style lang="scss" scoped>
.home {
  background: var(--bg-color);
}
</style>
