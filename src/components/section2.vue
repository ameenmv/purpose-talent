<template>
  <section class="pt-80 h-[100vh] section">
    <div class="flex flex-col justify-center items-center text">
      <h1
        class="text-[8.6vw] font-bold rotate-[-15deg] ml-[-12vw] h-[130px] items-center flex uppercase people"
      >
        people
      </h1>
      <h1
        class="text-[8.6vw] font-bold rotate-[4deg] ml-[-12vw] h-[130px] items-center flex uppercase ml-[200px] make"
      >
        make
      </h1>
      <h1
        class="text-[8.6vw] font-bold rotate-[-1deg] ml-[-12vw] h-[130px] items-center flex uppercase ml-[200px] businesses"
      >
        businesses
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
    // people ani
    gsap.fromTo(
      ".people",
      { opacity: 0, y: 50 },
      {
        opacity: 1,
        y: 0,
        scrollTrigger: {
          trigger: ".section",
          start: "top 20%",
          end: "top 0%",
          scrub: true,
          markers: true,
        },
      }
    );
    // make ani
    gsap.fromTo(
      ".make",
      { opacity: 0, y: 50 },
      {
        opacity: 1,
        y: 0,
        scrollTrigger: {
          trigger: ".section",
          start: "top 0%",
          end: "top -10%",
          scrub: true,
          markers: true,
        },
      }
    );
    gsap.fromTo(
      ".businesses",
      { opacity: 0, y: 50 },
      {
        opacity: 1,
        y: 0,
        scrollTrigger: {
          trigger: ".section",
          start: "top -10%",
          end: "top -20%",
          scrub: true,
          markers: true,
        },
      }
    );
    // pin text untill end
    gsap.to(".text", {
      scrollTrigger: {
        trigger: ".section",
        start: "top top",
        end: "bottom 0%",
        pin: true,
        toggleActions: "play none reverse none",
        markers: true,
      },
    });
    // businesses ani
  },
};
</script>
<!-- make the third word after pray -->
<style lang="scss" scoped></style>
