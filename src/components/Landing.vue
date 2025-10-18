<template>
  <section class="landing">
    <div class="containerr gap-3">
      <div class="flex justify-center items-center">
        <div class="left flex justify-center items-center w-[50%]">
          <img class="mb-[-40px]" src="../assets/man1.gif" alt="" />
        </div>
        <div class="right flex flex-col justify-center w-[50%] gap-[4vw]">
          <div class="flex flex-col mt-[-20px]">
            <h1
              class="text-[150px] font-bold rotate-[-2.2deg] ml-[-12vw] h-[130px] items-center flex uppercase relative afterr"
            >
              work
            </h1>
            <h1
              class="text-[150px] font-bold font-var(--cairo) rotate-[1.3deg] h-[130px] items-center flex uppercase"
            >
              that
            </h1>
            <h1
              class="text-[150px] font-bold rotate-[-1.9deg] h-[130px] items-center flex uppercase"
            >
              matters
            </h1>
          </div>
          <div class="flex flex-col gap-[1.1vw]">
            <p class="text-[16px] text-[var(--light-brown)]">
              Search + Talent Consultancy
            </p>
            <h2 class="text-[22px] font-semibold text-[var(--black)]">
              Connecting groundbreaking <br />
              companies with ordinary talent
            </h2>
            <div class="flex gap-[.8vw] mt-8">
              <button class="btn"><p>Learn More</p></button>
              <button
                class="btn !bg-[transparent] !text-[var(--light-brown)] borderr"
              >
                <p>Get in touch</p>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Landing",
};
</script>

<style lang="scss" scoped>
.landing {
  height: calc(100% - 75px);
  display: flex;
  align-items: center;
}
.borderr {
  border: 1px solid rgb(167, 151, 133);
}
.afterr::after {
  content: "";
  mix-blend-mode: darken;
  transform: rotateX(180deg) rotateY(0) rotateZ(57deg);
  display: block;
  width: 12vw;
  height: 12vw;
  background-image: url("../assets/landing.gif");
  background-size: cover;
  background-repeat: no-repeat;
  position: absolute;
  top: -15px;
  right: 315px;
}
h1 {
  font-family: var(--cairo);
}
</style>
