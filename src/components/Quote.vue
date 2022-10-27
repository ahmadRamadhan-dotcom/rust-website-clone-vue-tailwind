<template>
  <div
    id="funfact"
    class="bg-[#1b1b1b] mt-14 sm:mt-0 h-[70vh] sm:h-[60vh] md:h-[40vh] xl:h-[50vh] 2xl:h-[28vh] flex justify-center lg:-translate-y-32 md:-translate-y-60"
  >
    <div
      class="grid xl:w-[750px] text-center place-items-center place-content-center"
    >
      <p
        id="quote-text"
        class="font-['Bebas_Neue'] leading-[48px] sm:leading-[48px] w-10/12 sm:w-11/12 lg:w-10/12 xl:w-full xl:leading-[44px] relative text-[48px] font-medium text-[#e4dad1]"
      >
        “Rust is one of the cruelest games on Steam, and that's what makes it so
        compelling.”
      </p>
      <a
        href="https://www.pcgamer.com/uk/rust-review/"
        targer="_blank"
        class="text-2xl hover:text-[#cd412b] text-[#e4dad1] mt-14 sm:mt-12 xl:mt-14 font-['Bebas_Neue'] font-normal"
        >pc gamer</a
      >
    </div>
  </div>
</template>

<style scoped>
#quote-text::after {
  content: "";
  background: linear-gradient(
    to right,
    rgba(205, 65, 43, 0),
    #cd412b,
    rgba(205, 65, 43, 0)
  );
  position: absolute;
  bottom: -28px;
  left: 20%;
  right: 20%;
  height: 2px;
}
</style>
