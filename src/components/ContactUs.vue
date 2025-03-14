<template>
  <section class="px-4 lg:px-10 xl:px-0 flex flex-col">
    <div
      class="flex flex-col lg:flex-row items-center justify-center lg:justify-start gap-y-8 gap-x-10"
    >
      <h4
        class="bg-[#B9FF66] px-[7px] rounded-[7px] font-medium text-[36px] xl:text-[40px] text-black"
      >
        Contact Us
      </h4>
      <p
        class="lg:max-w-[323px] text-base xl:text-lg text-black font-normal text-center lg:text-left"
      >
        Connect with Us: Let's Discuss Your Digital Marketing Needs
      </p>
    </div>
    <div
      class="lg:my-20 mb-5 mt-10 bg-[#F3F3F3] rounded-[45px] py-10 px-5 lg:pl-[80px] xl:py-[60px] xl:pl-[100px] flex flex-col lg:flex-row xl:gap-x-20 justify-between"
    >
      <div class="basis-full lg:basis-[50%] flex flex-col">
        <form action="" class="lg:mb-10 flex flex-col gap-y-5 lg:gap-y-10">
          <div class="flex items-center justify-center lg:justify-start gap-x-10">
            <div class="flex items-center gap-x-[15px] lg:gap-x-5">
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
            class="text-white bg-[#191A23] text-xl py-5 px-[35px] justify-center rounded-[14px] lg:flex hidden"
          >
            Send Message
          </button>
        </form>
      </div>
      <div
        class="basis-full lg:basis-[50%] hidden lg:flex justify-end text-end"
      >
        <img
          src="/images/contact-image.svg"
          alt="image"
          class="relative lg:left-50 xl:left-60 2xl:left-65 w-[691.57px] h-[648px] lg:h-full lg:w-full aspect-[691.6/648]"
        />
      </div>
    </div>
    <button
      class="text-white bg-[#191A23] py-5 px-[35px] rounded-[14px] text-xl block lg:hidden mb-20"
    >
      Send Message
    </button>
  </section>
</template>
