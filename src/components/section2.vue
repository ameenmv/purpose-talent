<template>
  <section class="pt-80 h-[100vh] section2">
    <div class="flex flex-col justify-center items-center">
      <h1
        class="text-[8.6vw] font-bold rotate-[-15deg] ml-[-12vw] h-[130px] items-center flex uppercase people"
      >
        people
      </h1>
      <h1
        class="text-[8.6vw] font-bold rotate-[4deg] ml-[-12vw] h-[130px] items-center flex uppercase ml-[200px]"
      >
        make
      </h1>
    </div>
  </section>
</template>

<script>
import gsap from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";
gsap.registerPlugin(ScrollTrigger);
export default {
  mounted() {
    gsap.fromTo(
      ".people",
      { opacity: 0, y: 50 },
      {
        opacity: 1,
        y: 0,
        scrollTrigger: {
          trigger: ".section2",
          start: "top 20%",
          end: "top 0%",
          scrub: true,
          markers: true,
        },
      }
    );
  },
};
</script>

<style lang="scss" scoped></style>
