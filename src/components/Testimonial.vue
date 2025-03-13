<script>
export default {
  data() {
    return {
      testimonials: [
        {
          name: "John Smith",
          position: "Marketing Director at XYZ Corp",
          content:
            "We have been working with Positivus for the past year and have seen a significant increase in website traffic and leads as a result of their efforts. The team is professional, responsive, and truly cares about the success of our business. We highly recommend Positivus to any company looking to grow their online presence.",
        },
        {
          name: "John Smith",
          position: "Marketing Director at XYZ Corp",
          content:
            "We have been working with Positivus for the past year and have seen a significant increase in website traffic and leads as a result of their efforts. The team is professional, responsive, and truly cares about the success of our business. We highly recommend Positivus to any company looking to grow their online presence.",
        },
        {
          name: "John Smith",
          position: "Marketing Director at XYZ Corp",
          content:
            "We have been working with Positivus for the past year and have seen a significant increase in website traffic and leads as a result of their efforts. The team is professional, responsive, and truly cares about the success of our business. We highly recommend Positivus to any company looking to grow their online presence.",
        },
      ],
    };
  },
};
</script>

<template>
  <section class="px-4 lg:px-10 xl:px-0">
    <div
      class="flex flex-col lg:flex-row items-center justify-center xl:justify-start gap-y-8 gap-x-10"
    >
      <h4
        class="bg-[#B9FF66] px-[7px] rounded-[7px] font-medium text-[36px] xl:text-[40px] text-black"
      >
        Testimonials
      </h4>
      <p
        class="xl:max-w-[550px] text-base xl:text-lg text-black font-normal text-center lg:text-left"
      >
        Hear from Our Satisfied Clients: Read Our Testimonials to Learn More
        about Our Digital Marketing Services
      </p>
    </div>
    <div class="my-20 bg-[#191A23] px-5 lg:px-10 py-5 lg:py-20 pb-20 xl:pb-40 rounded-[45px]">
      <div class="overflow-x-auto flex gap-x-10 case-studies">
        <div class="flex flex-shrink-0" v-for="(item, index) in testimonials" :key="index">
          <div class="flex flex-col gap-y-5">
            <div
              class="border border-[#B9FF66] rounded-[45px] p-5 lg:p-10 max-w-[330px] lg:max-w-[606px] flex-shrink-0"
            >
              <p class="text-base xl:text-lg font-normal text-white">
                "We have been working with Positivus for the past year and have
                seen a significant increase in website traffic and leads as a
                result of their efforts. The team is professional, responsive,
                and truly cares about the success of our business. We highly
                recommend Positivus to any company looking to grow their online
                presence."
              </p>
            </div>
            <div class="ml-10 xl:ml-14 flex flex-col">
              <h4 class="text-[#B9FF66] text-base xl:text-lg font-normal">John Smith</h4>
              <p class="text-white text-base xl:text-lg font-normal">
                Marketing Director at XYZ Corp
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
