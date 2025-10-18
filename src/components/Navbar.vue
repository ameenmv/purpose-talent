<template>
  <div class="w-[100%] flex justify-between pl-6 pr-6 pt-3 pb-3">
    <div class="flex gap-4">
      <div class="flex cursor-pointer tele items-center rounded-[30px] p-2">
        <img class="w-[30px]" src="../assets/telescope.svg" alt="" />
        <p class="font-semibold pl-4 pr-4">Companies</p>
      </div>
      <div class="flex cursor-pointer tele items-center rounded-[30px] p-2">
        <img class="w-[30px]" src="../assets/candidates.svg" alt="" />
        <p class="font-semibold pl-4 pr-4">Candidates</p>
      </div>
    </div>
    <div class="logo">
      <img class="w-[120px]" src="../assets/logo.svg" alt="" />
    </div>
    <div class="flex gap-8 items-center">
      <p class="font-semibold">New York | 8:48 am</p>
      <div
        class="flex cursor-pointer tele contact items-center rounded-[30px] p-2"
      >
        <img class="w-[30px]" src="../assets/message.svg" alt="" />
        <p class="font-semibold pl-4 pr-4">Contact</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style lang="scss" scoped>
.tele {
  background: #f0e4d6;
}
.tele p {
  color: var(--black);
  opacity: 0.8;
}
p {
  color: var(--black);
}
.contact {
  background: var(--black);
}
.contact p {
  color: var(--white);
}
</style>
