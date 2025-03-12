<template>
  <section class="px-4 xl:px-0 flex flex-col">
    <div
      class="flex flex-col xl:flex-row items-center justify-center xl:justify-start gap-y-8 gap-x-10"
    >
      <h4
        class="bg-[#B9FF66] px-[7px] rounded-[7px] font-medium text-[36px] xl:text-[40px] text-black"
      >
        Contact Us
      </h4>
      <p
        class="xl:max-w-[323px] text-base xl:text-lg text-black font-normal text-center xl:text-left"
      >
        Connect with Us: Let's Discuss Your Digital Marketing Needs
      </p>
    </div>
    <div
      class="xl:my-20 mb-5 mt-10 bg-[#F3F3F3] rounded-[45px] py-10 px-5 xl:py-[60px] xl:pl-[100px] flex flex-col xl:flex-row gap-x-20 justify-between"
    >
      <div class="basis-full xl:basis-[50%] flex flex-col">
        <form action="" class="xl:mb-10 flex flex-col gap-y-5 xl:gap-y-10">
          <div class="flex items-center justify-center xl:justify-start gap-x-10">
            <div class="flex items-center gap-x-[15px] xl:gap-x-5">
              <input
                type="radio"
                name="contact-option"
                id=""
                class="accent-[#B9FF66] w-7 h-7"
              />
              <span class="text-base xl:text-lg text-black font-normal">Say Hi</span>
            </div>
            <div class="flex items-center gap-x-[15px] xl:gap-x-5">
              <input
                type="radio"
                name="contact-option"
                id=""
                class="accent-[#B9FF66] w-7 h-7"
              />
              <span class="text-base xl:text-lg text-black font-normal">Get a Quote</span>
            </div>
          </div>

          <div class="flex flex-col gap-y-[5px]">
            <label for="" class="text-base text-black font-normal">Name</label>
            <input
              type="text"
              placeholder="Name"
              class="border border-black bg-white py-4.5 px-5 xl:px-[30px] text-base xl:text-lg rounded-[14px]"
            />
          </div>
          <div class="flex flex-col gap-y-[5px]">
            <label for="" class="text-base text-black font-normal"
              >Email*</label
            >
            <input
              type="email"
              name="email"
              placeholder="Email"
              class="border border-black bg-white py-4.5 px-5 xl:px-[30px] text-base xl:text-lg rounded-[14px]"
            />
          </div>
          <div class="flex flex-col gap-y-[5px]">
            <label for="" class="text-base text-black font-normal">Message*</label>
            <textarea
              type="text"
              placeholder="Message"
              name="message"
              class="border border-black bg-white py-4.5 px-5 xl:px-[30px] text-base xl:text-lg rounded-[14px] resize-none h-[190px]"
            />
          </div>
          <button
            class="text-white bg-[#191A23] text-xl py-5 px-[35px] rounded-[14px] xl:flex hidden"
          >
            Send Message
          </button>
        </form>
      </div>
      <div
        class="basis-full xl:basis-[50%] hidden xl:flex justify-end text-end"
      >
        <img
          src="/images/contact-image.svg"
          alt="image"
          class="relative xl:left-60 2xl:left-65 w-[691.57px] h-[648px]"
        />
      </div>
    </div>
    <button
      class="text-white bg-[#191A23] py-5 px-[35px] rounded-[14px] text-xl block xl:hidden mb-20"
    >
      Send Message
    </button>
  </section>
</template>
