<template>
  <div id="banner-hero" class="relative 2xl:mx-auto bg-[#141312] md:-z-[10]">
    <div
      :class="{
        'opacity-[0.8675] blur-[3.975px] xl:opacity-[1] xl:blur-[0px]':
          scrollPosition > 40,
        'opacity-[0.6025] blur-[11.925px] xl:opacity-[0.6025] xl:blur-[11.925px]':
          scrollPosition > 80,
        'opacity-[0.1175] blur-[26.475px] xl:opacity-[0.1175]':
          scrollPosition > 350,
        'opacity-[0.1] blur-[30px]': scrollPosition > 450,
      }"
      class="hero-video sm:pb-60 transition-header"
    >
      <video
        id="myVideo"
        autoplay="true"
        muted="true"
        loop="true"
        playsinline="true"
        class="md:w-full md:h-[700px] 2xl:h-[1000px] md:object-cover md:-z-[100]"
      >
        <source
          src="https://files.facepunch.com/paddy/20210324/rust_site2021_hero_v002.mp4"
          type="video/mp4"
        />
      </video>
    </div>
    <div
      class="wrapper absolute sm:top-24 md:top-60 lg:top-24 sm:left-10 lg:left-0 xl:left-32 2xl:left-0 2xl:right-0 2xl:bottom-0 2xl:top-40 2xl:w-[1100px] 2xl:m-auto"
    >
      <h1
        class="font-['Bebas_Neue'] sm:w-72 xl:w-72 leading-[80px] sm:leading-[80px] lg:leading-[160px] text-[96px] sm:text-[96px] lg:text-[192px] 2xl:text-[12rem] text-[#e4dad1] font-medium"
      >
        Explore Build Survive
      </h1>
      <p
        class="text-base text-[#e4dad1] mt-5 sm:mt-0 xl:mt-5 font-normal font-['Open_Sans'] mb-7 sm:mb-5 lg:mb-7 xl:mb-8 sm:w-[96%] lg:w-6/12 xl:w-[550px]"
      >
        The only aim in Rust is to survive. Everything wants you to die - the
        island’s wildlife and other inhabitants, the environment, other
        survivors. Do whatever it takes to last another night.
      </p>
      <div class="flex sm:flex gap-3 sm:gap-3 xl:gap-4">
        <a
          href="https://rust.facepunch.com/buy"
          target="_blank"
          class="py-1.5 px-4 sm:py-1.5 xl:py-1 sm:px-4 xl:px-5 text-[#ffffff] bg-[#cd412b] text-[24px] sm:text-[24px] lg:text-[28px] font-normal font-['Bebas_Neue']"
          >buy rust</a
        >
        <a
          href="https://www.youtube.com/watch?v=LGcECozNXEw"
          class="bg-[#2a2928] px-5 sm:px-5 xl:px-4 py-1 sm:py-1 xl:py-1 border text-[#e4dad1] text-[24px] sm:text-[24px] lg:text-[28px] font-normal font-['Bebas_Neue']"
          target="_blank"
          >watch trailer</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BannerHero",
  data() {
    return {
      scrollPosition: null,
    };
  },
  methods: {
    updateScroll() {
      this.scrollPosition = window.scrollY;
    },
  },
  mounted() {
    window.addEventListener("scroll", this.updateScroll);
  },
};
</script>

<style scoped>
@media (max-width: 639px) {
  #myVideo {
    width: full;
    height: 100vh;
    object-fit: cover;
  }
  .wrapper {
    top: 230px;
    left: 0;
    right: 0;
    bottom: 0;
    margin: auto;
    width: 83.333333%;
  }
}
</style>
