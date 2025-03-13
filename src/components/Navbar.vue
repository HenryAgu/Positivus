<script>
export default {
  data() {
    return {
      openMenu: false,
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
  methods:{
    handleOpenMenu(){
      this.openMenu = true;
    },
    handleCloseMenu(){
      this.openMenu = false;
    }
  }
};
</script>

<template>
  <header
    class="flex items-center justify-between px-4 lg:px-8 xl:px-0 py-6 xl:pt-10 2xl:pt-14"
  >
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
    <div class="hidden lg:flex items-center flex-row lg:gap-x-5 xl:gap-x-10">
      <ul class="flex flex-row lg:gap-x-5 xl:gap-x-10">
        <li v-for="item in menu" :key="item.id">
          <span class="text-black font-normal text-xl"> {{ item.title }} </span>
        </li>
      </ul>
      <button
        class="border border-[#191A23] bg-white hover:bg-[#B9FF66] duration-200 ease-in-out transition cursor-pointer py-3.5 px-[35px] rounded-[14px] text-black text-xl font-weight"
      >
        Request a quote
      </button>
    </div>
    <div class="flex lg:hidden">
      <button @click="handleOpenMenu">
        <img src="../assets/images/menu.svg" alt="Logo" class="w-6 h-4" />
      </button>
    </div>

    <!-- Mobile Menu -->
    <Transition
      mode="out-in"
      enter-active-class="transition-all duration-200 ease-out"
      leave-active-class="transition-all duration-250 ease-in"
    >
      <div
      v-if="openMenu"
        class="fixed top-0 left-0 right-0 bg-white h-fit p-5 pb-10 flex lg:hidden flex-col gap-y-5 shadow-2xl"
      >
        <div class="flex justify-end">
          <button @click="handleCloseMenu"><i class="pi pi-times" style="font-size: 1.5rem"></i></button>
        </div>
        <p class="font-medium text-[30px] text-black">
          Check out my <br> portfolio! ;)
        </p>
        <a href="https://henry-agu.vercel.app/" target="_blank"
          class="bg-[#B9FF66] py-5 px-[35px] text-center rounded-[14px] w-full underline text-black font-normal"
        >
          Go to Henry's website
        </a>
      </div>
    </Transition>
  </header>
</template>
