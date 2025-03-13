<script>
import { Transition } from 'vue';

export default {
  data() {
    return {
      bgColor: "#F3F3F3",
      faqs: [
        {
          title: "Consultation",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
          isActive: true,
        },
        {
          title: "Research and Strategy Development",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
          isActive: false,
        },
        {
          title: "Implementation",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
          isActive: false,
        },
        {
          title: "Monitoring and Optimization",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
          isActive: false,
        },
        {
          title: "Reporting and Communication",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
          isActive: false,
        },
        {
          title: "Continual Improvement",
          content:
            "During the initial consultation, we will discuss your business goals and objectives, target audience, and current marketing efforts. This will allow us to understand your needs and tailor our services to best fit your requirements.",
          isActive: false,
        },
      ],
    };
  },
  methods: {
    toggleFaq(index) {
      this.faqs[index].isActive = !this.faqs[index].isActive;
    },
  },
};
</script>

<template>
  <section class="my-14 flex flex-col gap-y-5">
    <div class="" v-for="(faq, index) in faqs" :key="index">
      <div
        :class="`border-[#191A23] border p-[30px] lg:p-10 rounded-[45px] shadow-[0px_5px_0px_0px_#191A23]`"
        :style="{ backgroundColor: faq.isActive ? '#B9FF66' : '#F3F3F3' }"
      >
        <div class="flex items-center justify-between">
          <div class="flex items-center gap-x-3 lg:gap-x-[25px]">
            <h2 class="text-black text-[30px] lg:text-[60px] font-medium">
              0{{ index + 1 }}
            </h2>
            <p
              class="text-lg lg:text-[30px] text-black font-medium max-w-[203px] lg:max-w-full"
            >
              {{ faq.title }}
            </p>
          </div>
          <div class="">
            <button @click="toggleFaq(index)">
              <img
                :src="
                  faq.isActive
                    ? '/images/Minus-circle.svg'
                    : '/images/Plus-circle.svg'
                "
                alt="icon"
                class="h-[30px] w-[30px] lg:w-[58px] lg:h-[58px] cursor-pointer"
              />
            </button>
          </div>
        </div>
        <Transition
          name="faq"
          mode="out-in"
          enter-active-class="transition-all duration-200 ease-out"
          leave-active-class="transition-all duration-250 ease-in"
          enter-from-class="opacity-0 max-h-0"
          enter-to-class="opacity-100 max-h-[500px]"
          leave-from-class="opacity-100 max-h-[500px]"
          leave-to-class="opacity-0 max-h-0"
        >
          <div v-if="faq.isActive" class="border-t border-black pt-5">
            <p class="text-lg text-black font-normal">{{ faq.content }}</p>
          </div>
        </Transition>
      </div>
    </div>
  </section>
</template>
