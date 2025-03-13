<template>
  <footer class="bg-[#191A23] px-5 py-10 lg:p-10 lg:rounded-tl-[45px] lg:rounded-tr-[45px] w-full">
    <div class="">
      <div class="flex flex-col lg:flex-row items-center justify-between">
        <div class="">
          <img
            src="../assets/images/Logo-white.svg"
            alt="Logo"
            class="h-[23.01px] w-[139.89px]"
          />
        </div>
        <div class="flex items-center flex-row gap-x-10 mt-10 lg:mt-0">
          <ul class="flex flex-col items-center lg:flex-row gap-x-10 gap-y-3.5">
            <li v-for="(item, index) in menu" :key="index">
              <span
                class="text-white lg:underline font-normal text-base lg:text-lg"
              >
                {{ item.title }}
              </span>
            </li>
          </ul>
        </div>
        <div class="hidden md:flex flex-row items-center gap-x-5">
          <div class="" v-for="(item, index) in social" :key="index">
            <img
              :src="item.image"
              alt="social-media-icon"
              class="w-[30px] h-[30px]"
            />
          </div>
        </div>
      </div>
      <div
        class="mt-20 flex flex-col lg:flex-row items-center gap-x-20 gap-y-10 border-b border-white pb-10 w-full"
      >
        <div class="flex flex-col items-center lg:items-start lg:text-left text-center gap-y-3 lg:gap-y-5 basis-full lg:basis-[40%]">
          <span
            class="text-black w-fit xl:py-1 px-2 xl:px-3 rounded-[7px] bg-[#B9FF66] font-medium text-lg xl:text-2xl mb-5 xl:mb-0"
            >Contact us:</span
          >
          <p class="text-white text-base lg:text-lg font-normal">
            Email: info@positivus.com
          </p>
          <p class="text-white text-base lg:text-lg font-normal">Phone: 555-567-8901</p>
          <p class="text-white text-base lg:text-lg font-normal">
            Address: 1234 Main St <br />
            Moonstone City, Stardust State 12345
          </p>
        </div>
        <div class="basis-full lg:basis-[80%] xl:basis-[60%]">
          <div
            class="bg-[#292A32] p-[30px] xl:px-10 xl:py-[58px] rounded-[14px] flex lg:flex-row flex-col gap-5"
          >
            <input
              type="text"
              placeholder="Email"
              class="border border-white py-5 lg:py-[22px] px-[25px] lg:px-[35px] rounded-[14px] lg:basis-[50%] text-white text-lg outline-transparent"
            />
            <button
              class="bg-[#B9FF66] w-full rounded-[14px] py-5 lg:py-[22px] px-[25px] lg:px-[5px] text-black text-xl font-normal lg:basis-[50%]"
            >
              Subscribe to news
            </button>
          </div>
        </div>
      </div>
      <div class="mt-10 flex flex-col lg:flex-row items-center gap-y-3.5 gap-x-10">
        <p class="text-white text-base xl:text-lg font-normal">
          © 2023 Positivus. All Rights Reserved.
        </p>
        <p class="text-white text-base xl:text-lg font-normal underline">Privacy Policy</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      menu: [
        {
          title: "About us",
          link: "/about",
        },
        {
          title: "Services",
          link: "/about",
        },
        {
          title: "Use Cases",
          link: "/about",
        },
        {
          title: "Pricing",
          link: "/about",
        },
        {
          title: "Blog",
          link: "/about",
        },
      ],

      social: [
        {
          image: "/images/Linkedin.svg",
          path: "",
        },
        {
          image: "/images/Facebook.svg",
          path: "",
        },
        {
          image: "/images/X.svg",
          path: "",
        },
      ],
    };
  },
};
</script>
