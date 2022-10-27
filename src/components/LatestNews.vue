<template>
  <div id="latest-news" class="flex justify-center">
    <div class="grid place-content-center place-items-center">
      <div id="section-header" class="xl:w-[1060px] xl:translate-y-3">
        <p
          class="font-['Bebas_Neue'] text-xl flex gap-3 justify-center items-center font-medium w-[140px] h-10 text-center text-[#e4dad1] bg-[#cd412b]"
        >
          <span class="material-symbols-outlined"> feed </span>
          latest news
        </p>
      </div>
      <figure class="xl:w-[1100px]">
        <img src="../assets/Ko-YNOaE.jpg" alt="latest news image" />
      </figure>
      <div
        class="xl:w-[890px] 2xl:w-[800px] grid place-items-center bg-[#1f1f1f] xl:h-[65vh] 2xl:h-[350px] 2xl:pb-3 xl:-translate-y-24"
      >
        <span
          id="title"
          class="font-['Bebas_Neue'] xl:text-[64px] text-[#e4dad1] font-medium"
        >
          <a
            href="https://rust.facepunch.com/news/halloween-2022"
            target="_blank"
            >halloween 2022</a
          >
        </span>
        <div
          class="tags-days w-[800px] relative xl:flex xl:justify-center xl:gap-3"
        >
          <p
            class="font-['Bebas_Neue'] z-[30] bg-[#cd412b] xl:py-1.5 xl:px-4 font-normal text-sm text-[#e4dad1]"
          >
            7 days ago
          </p>
          <a
            href="https://rust.facepunch.com/news/?category=devblog"
            target="_blank"
            class="font-['Bebas_Neue'] z-[30] bg-[#cd412b] xl:py-1.5 xl:px-4 font-normal text-sm text-[#e4dad1]"
          >
            devblog
          </a>
        </div>
        <p
          class="font-['Open_Sans'] xl:w-[600px] text-center font-normal text-base text-[#bab1a8]"
        >
          A darkness is falling upon Rust, monsters are awakening, portals are
          opening, and skulls are breaking. Enter if you dare.
        </p>
        <a
          href="https://rust.facepunch.com/news/halloween-2022"
          target="_blank"
          class="font-['Bebas_Neue'] font-normal text-[#ffffff] text-xl bg-[#cd412b] xl:py-1.5 xl:px-4"
          >read more</a
        >
      </div>
    </div>
  </div>
</template>

<style scoped>
.tags-days::before {
  content: "";
  background: linear-gradient(
    to right,
    rgba(205, 65, 43, 0),
    #cd412b,
    rgba(205, 65, 43, 0)
  );
  position: absolute;
  bottom: 50%;
  left: 20%;
  right: 20%;
  height: 2px;
  transform: translateY(-50%);
}
</style>
