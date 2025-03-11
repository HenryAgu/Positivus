<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default {
  components: {
    Navbar,
    Footer,
  },
};
</script>

<template>
  <main class="container w-full mx-auto px-0 xl:px-10 2xl:px-14 bg-white">
    <Navbar />
    <main class="min-h-screen">
      <!-- Hero -->
      <section class="my-5 xl:my-10 flex flex-col-reverse gap-y-5 xl:flex-row justify-between px-4 xl:px-0">
        <div class="basis-full xl:basis-[50%] flex flex-col gap-y-[35px]">
          <h1 class="text-black font-medium text-[60px] leading-[70px] hidden xl:block">
            Navigating the <br />
            digital landscape <br />
            for success
          </h1>
          <p
            class="text-base xl:text-xl font-normal text-black max-w-[498px] leading-[24px] xl:leading-[28px]"
          >
            Our digital marketing agency helps businesses grow and succeed
            online through a range of services including SEO, PPC, social media
            marketing, and content creation.
          </p>
          <button
            class="w-full xl:w-fit bg-[#191A23] rounded-[14px] text-white font-normal text-xl py-5 px-[35px]"
          >
            Book a consultation
          </button>
        </div>
        <div class="basis-full xl:basis-[50%] flex justify-center xl:justify-end">
          <img
            src="/images/Hero.png"
            alt="hero-image"
            class="w-[361.44px] h-[310px] xl:w-[600.46px] xl:h-[515px]"
          />
        </div>
        <h1 class="text-black font-medium text-[43px] leading-[55px] block xl:hidden">
            Navigating the <br />
            digital landscape <br />
            for success
          </h1>
      </section>
    </main>
    <Footer />
  </main>
</template>
