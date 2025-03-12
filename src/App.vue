<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import Services from "@/components/Services.vue";
import Faq from "@/components/Faq.vue";
import Team from "@/components/Team.vue";

export default {
  components: {
    Navbar,
    Footer,
    Services,
    Faq,
    Team,
  },
  data() {
    return {
      brands: [
        {
          id: crypto.randomUUID(),
          image: "/images/Amazon.svg",
        },
        {
          id: crypto.randomUUID(),
          image: "/images/Dribble.svg",
        },
        {
          id: crypto.randomUUID(),
          image: "/images/Hubspot.svg",
        },
        {
          id: crypto.randomUUID(),
          image: "/images/Notion.svg",
        },
        {
          id: crypto.randomUUID(),
          image: "/images/Netflix.svg",
        },
        {
          id: crypto.randomUUID(),
          image: "/images/Zoom.svg",
        },
      ],
      caseStudies: [
        {
          content:
            "For a local restaurant, we implemented a targeted PPC campaign that resulted in a 50% increase in website traffic and a 25% increase in sales.",
          path: "",
        },
        {
          content:
            "For a B2B software company, we developed an SEO strategy that resulted in a first page ranking for key keywords and a 200% increase in organic traffic.",
          path: "",
        },
        {
          content:
            "For a national retail chain, we created a social media marketing campaign that increased followers by 25% and generated a 20% increase in online sales.",
          path: "",
        },
      ],
    };
  },
};
</script>

<template>
  <main class="container w-full mx-auto px-0 xl:px-10 2xl:px-14 bg-white">
    <Navbar />
    <main class="min-h-screen">
      <!-- Hero -->
      <section
        class="my-5 xl:my-10 flex flex-col-reverse gap-y-5 xl:flex-row justify-between px-4 xl:px-0"
      >
        <div class="basis-full xl:basis-[50%] flex flex-col gap-y-[35px]">
          <h1
            class="text-black font-medium text-[60px] leading-[70px] hidden xl:block"
          >
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
        <div
          class="basis-full xl:basis-[50%] flex justify-center xl:justify-end"
        >
          <img
            src="/images/Hero.png"
            alt="hero-image"
            class="w-[361.44px] h-[310px] xl:w-[600.46px] xl:h-[515px]"
          />
        </div>
        <h1
          class="text-black font-medium text-[43px] leading-[55px] block xl:hidden"
        >
          Navigating the <br />
          digital landscape <br />
          for success
        </h1>
      </section>

      <!-- Brands -->
      <section
        class="flex flex-wrap xl:flex-nowrap items-center justify-center gap-x-10 gap-y-2.5 xl:justify-between my-14"
      >
        <div class="" v-for="item in brands" :key="item.id">
          <img :src="item.image" alt="brand" class="grayscale h-12" />
        </div>
      </section>

      <!-- Services -->
      <section class="my-20 px-4 xl:px-0">
        <div
          class="flex flex-col xl:flex-row items-center justify-center xl:justify-start gap-y-8 gap-x-10"
        >
          <h4
            class="bg-[#B9FF66] px-[7px] rounded-[7px] font-medium text-[36px] xl:text-[40px] text-black"
          >
            Services
          </h4>
          <p
            class="xl:max-w-[550px] text-base xl:text-lg text-black font-normal text-center xl:text-left"
          >
            At our digital marketing agency, we offer a range of services to
            help businesses grow and succeed online. These services include:
          </p>
        </div>
        <Services />
      </section>

      <!-- Proposal banner -->
      <section class="relative px-4 xl:px-0">
        <div class="bg-[#F3F3F3] rounded-[45px] my-20 flex">
          <div
            class="p-[50px] xl:p-[60px] flex flex-col gap-y-5 basis-full xl:basis-[50%]"
          >
            <h3 class="text-black text-[26px] xl:text-[30px] font-medium">
              Let’s make things happen
            </h3>
            <p
              class="text-black font-normal text-base xl:text-lg xl:max-w-[550px] leading-[28px] xl:leading-[30px]"
            >
              Contact us today to learn more about how our digital marketing
              services can help your business grow and succeed online.
            </p>
            <button
              class="w-full xl:w-fit bg-[#191A23] text-lg xl:text-xl text-white py-5 xl:px-[35px] rounded-[14px]"
            >
              Get your free proposal
            </button>
          </div>
        </div>
        <div
          class="hidden xl:flex justify-end mr-32 -mb-[280px] relative bottom-110"
        >
          <img
            src="/images/banner1.png"
            alt="banner"
            class="w-[359px] h-[394.27px]"
          />
        </div>
      </section>

      <!-- Case studies -->
      <section class="px-4 xl:px-0">
        <div
          class="flex flex-col xl:flex-row items-center justify-center xl:justify-start gap-y-8 gap-x-10"
        >
          <h4
            class="bg-[#B9FF66] px-[7px] rounded-[7px] font-medium text-[36px] xl:text-[40px] text-black"
          >
            Case Studies
          </h4>
          <p
            class="xl:max-w-[550px] text-base xl:text-lg text-black font-normal text-center xl:text-left"
          >
            Explore Real-Life Examples of Our Proven Digital Marketing Success
            through Our Case Studies
          </p>
        </div>

        <!-- Desktop -->
        <div
          class="my-10 xl:my-20 bg-[#191A23] rounded-[45px] p-10 py-20 hidden xl:grid grid-cols-3"
        >
          <div
            v-for="(item, index) in caseStudies"
            :key="index"
            :class="[
              'px-10 flex flex-col gap-y-5',
              index !== caseStudies.length - 1 ? 'border-r border-white' : '',
            ]"
          >
            <p class="text-white text-lg font-normal">
              {{ item.content }}
            </p>
            <a href="" class="flex items-center gap-x-[15px]">
              <span class="text-[#B9FF66] text-xl font-normal">Learn more</span>
              <img src="/images/green-arrow.svg" alt="arrow_icon" />
            </a>
          </div>
        </div>

        <!-- Mobile -->
        <div
          class="my-10 flex xl:hidden items-center gap-x-5 overflow-x-auto case-studies"
        >
          <div
            class="flex-shrink-0"
            v-for="(item, index) in caseStudies"
            :key="index"
          >
            <div
              class="bg-[#191A23] rounded-[45px] px-[50px] py-[42px] flex flex-col gap-y-5 flex-shrink-0 max-w-[350px]"
            >
              <p class="text-base text-white font-normal leading-[24px]">
                {{ item.content }}
              </p>
              <a :href="item.path" class="flex items-center gap-x-[15px]"
                ><span class="text-[#B9FF66] text-xl font-normal"
                  >Learn more</span
                ><img src="/images/green-arrow.svg" alt="arrow_icon"
              /></a>
            </div>
          </div>
        </div>
      </section>

      <!-- Working process -->
      <section class="px-4 xl:px-0 my-20">
        <div
          class="flex flex-col xl:flex-row items-center justify-center xl:justify-start gap-y-8 gap-x-10"
        >
          <h4
            class="bg-[#B9FF66] px-[7px] rounded-[7px] font-medium text-[36px] xl:text-[40px] text-black hidden xl:block"
          >
            Our Working Process
          </h4>
          <div class="flex xl:hidden flex-col items-center">
            <h4
              class="bg-[#B9FF66] px-[7px] rounded-[7px] font-medium text-[36px] xl:text-[40px] text-black w-fit"
            >
              Our Working
            </h4>
            <h4
              class="bg-[#B9FF66] px-[7px] rounded-[7px] font-medium text-[36px] xl:text-[40px] text-black w-fit"
            >
              Process
            </h4>
          </div>
          <p
            class="xl:max-w-[292px] text-base xl:text-lg text-black font-normal text-center xl:text-left"
          >
            Step-by-Step Guide to Achieving Your Business Goals
          </p>
        </div>
        <Faq />
      </section>

      <!-- Teams -->
      <section class="px-4 xl:px-0">
        <div
          class="flex flex-col xl:flex-row items-center justify-center xl:justify-start gap-y-8 gap-x-10"
        >
          <h4
            class="bg-[#B9FF66] px-[7px] rounded-[7px] font-medium text-[36px] xl:text-[40px] text-black"
          >
            Team
          </h4>
          <p
            class="xl:max-w-[550px] text-base xl:text-lg text-black font-normal text-center xl:text-left"
          >
            Meet the skilled and experienced team behind our successful digital
            marketing strategies
          </p>
        </div>
        <Team/>
      </section>
    </main>
    <Footer />
  </main>
</template>
