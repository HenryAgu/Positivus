<script>
export default {
  data() {
    return {
      faqs: [
        {
          title: "Consultation",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
        },
        {
          title: "Research and Strategy Development",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
        },
        {
          title: "Implementation",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
        },
        {
          title: "Monitoring and Optimization",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
        },
        {
          title: "Reporting and Communication",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
        },
        {
          title: "Continual Improvement",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
        },
      ],
    };
  },
};
</script>

<template>
  <section class="my-20 flex flex-col gap-y-5">
    <div class="" v-for="(faq, index) in faqs" :key="index">
      <div
        class="border-[#191A23] border bg-[#F3F3F3] p-[30px] lg:p-10 rounded-[45px] shadow-[0px_5px_0px_0px_#191A23]"
      >
        <div class="flex items-center justify-between pb-5 lg:pb-0">
          <div class="flex items-center gap-x-3 lg:gap-x-[25px]">
            <h2 class="text-black text-[30px] lg:text-[60px] font-medium">0{{ index + 1 }}</h2>
            <p class="text-lg lg:text-[30px] text-black font-medium max-w-[203px] lg:max-w-full">{{ faq.title }}</p>
          </div>
          <div class="">
            <button><img src="/images/Plus-circle.svg" alt="icon" class="h-[30px] w-[30px] lg:w-[58px] lg:h-[58px]"/></button>
          </div>
        </div>
        <div class="border-t border-black pt-5">
          <p class="text-lg text-black font-normal">{{ faq.content }}</p>
        </div>
      </div>
    </div>
  </section>
</template>
