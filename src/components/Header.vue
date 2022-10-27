<template>
  <header
    class="flex justify-center bg-[#151413] z-[999] md:translate-y-[140px] lg:translate-y-0 2xl:translate-y-[70px] h-0 sm:h-[27vh] md:h-0 lg:h-[9vh] xl:h-[11vh] 2xl:h-0"
  >
    <div
      class="lg:w-[950px] xl:w-[1100px] sm:pb-1 md:pb-0 sm:grid z-[30] sm:place-content-end sm:place-items-center lg:flex lg:justify-between sm:items-end"
    >
      <figure>
        <img
          src="../assets/rust-marque.svg"
          alt="rust header logo"
          class="translate-y-8 translate-x-32 sm:translate-x-0 sm:-translate-y-6 lg:translate-y-1 xl:translate-y-2"
        />
      </figure>
      <div
        class="flex gap-5 sm:flex sm:gap-6 lg:gap-7 xl:gap-9 sm:translate-y-5 lg:translate-y-0"
      >
        <p
          id="content"
          class="text-[#e4dad1] translate-y-[90px] sm:translate-y-0 font-['Bebas_Neue'] font-medium text-xl sm:text-xl lg:translate-y-3 xl:translate-y-3"
          v-for="(data, index) in headerList"
          :key="index"
        >
          {{ data.name }}
        </p>
        <a
          href="https://rust.facepunch.com/buy/"
          target="_blank"
          class="translate-y-20 sm:-translate-y-1 lg:translate-y-2 xl:translate-y-1 py-1.5 px-2 sm:py-1.5 sm:px-2 xl:py-1.5 xl:px-3 bg-[#cd412b] font-['Bebas_Neue'] font-medium text-xl sm:text-xl"
        >
          <p class="text-[#e4dad1]">buy rust</p>
        </a>
      </div>
    </div>
  </header>
</template>

<script setup>
const headerList = [
  { id: 1, name: "news" },
  { id: 2, name: "companion" },
  { id: 3, name: "official skins" },
];
</script>

<style scoped></style>
