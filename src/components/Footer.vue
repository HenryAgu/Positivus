<template>
  <footer class="bg-[#191A23] p-10 rounded-tl-[45px] rounded-tr-[45px]">
    <div>
      <div class="flex flex-row items-center justify-between">
        <div class="">
          <img
            src="../assets/images/Logo-white.svg"
            alt="Logo"
            class="h-[23.01px] w-[139.89px]"
          />
        </div>
        <div class="flex items-center flex-row gap-x-10">
          <ul class="flex flex-row gap-x-10">
            <li v-for="(item, index) in menu" :key="index">
              <span class="text-white underline font-normal text-lg">
                {{ item.title }}
              </span>
            </li>
          </ul>
        </div>
        <div class="flex flex-row items-center gap-x-5">
          <div class="" v-for="(item, index) in social" :key="index">
            <img
              :src="item.image"
              alt="social-media-icon"
              class="w-[30px] h-[30px]"
            />
          </div>
        </div>
      </div>
      <div class="mt-20 flex flex-row items-center gap-x-20 border-b border-white pb-10">
        <div class="flex flex-col gap-y-5 basis-[40%]">
          <span
            class="text-black w-fit py-1 px-3 rounded-[7px] bg-[#B9FF66] font-medium text-2xl"
            >Contact us:</span
          >
          <p class="text-white text-lg font-normal">
            Email: info@positivus.com
          </p>
          <p class="text-white text-lg font-normal">Phone: 555-567-8901</p>
          <p class="text-white text-lg font-normal">
            Address: 1234 Main St <br />
            Moonstone City, Stardust State 12345
          </p>
        </div>
        <div class="basis-[60%]">
          <div class="bg-[#292A32] px-10 py-[58px] rounded-[14px] flex gap-x-5">
            <input
              type="text"
              placeholder="Email"
              class="border border-white py-[22px] px-[35px] rounded-[14px] basis-[50%] text-white text-lg outline-transparent"
            />
            <button class="bg-[#B9FF66] w-full rounded-[14px] text-black text-xl font-normal basis-[50%]">Subscribe to news</button>
          </div>
        </div>
      </div>
      <div class="mt-10 flex items-center gap-x-10">
      <p class="text-white text-lg font-normal">© 2023 Positivus. All Rights Reserved.</p>
      <p class="text-white text-lg font-normal underline">Privacy Policy</p>
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
