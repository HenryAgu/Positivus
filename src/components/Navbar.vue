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
    };
  },
};
</script>

<template>
  <header class="flex items-center justify-between px-4 py-6 xl:pt-10 2xl:pt-14">
    <img
      src="../assets/images/Logo.svg"
      alt="Logo"
      class="h-[56px] w-[219.54px] hidden xl:block"
    />
    <img
      src="../assets/images/Mobile-logo.svg"
      alt="Logo"
      class="h-[23.61px] w-[144px] xl:hidden block"
    />
    <div class="hidden xl:flex items-center flex-row gap-x-10">
      <ul class="flex flex-row gap-x-10">
        <li v-for="item in menu" :key="item.id">
          <span class="text-black font-normal text-xl"> {{ item.title }} </span>
        </li>
      </ul>
      <button
        class="border border-[#191A23] py-3.5 px-[35px] rounded-[14px] text-black text-xl font-weight"
      >
        Request a quote
      </button>
    </div>
    <div class="flex xl:hidden">
      <button>
        <img src="../assets/images/menu.svg" alt="Logo" class="w-6 h-4" />
      </button>
    </div>
  </header>
</template>
