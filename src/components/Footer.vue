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
            <img :src="item.image" alt="social-media-icon" class="w-[30px] h-[30px]"/>
          </div>
        </div>
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
