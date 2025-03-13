<script>
export default {
  data() {
    return {
      teams: [
        {
          image: "/images/Picture.png",
          name: "John Smith",
          position: "CEO and Founder",
          content:
            "10+ years of experience in digital marketing. Expertise in SEO, PPC, and content strategy",
        },
        {
          image: "/images/Picture-1.png",
          name: "Jane Doe",
          position: "Director of Operations",
          content:
            "7+ years of experience in project management and team leadership. Strong organizational and communication skills",
        },
        {
          image: "/images/Picture-2.png",
          name: "Michael Brown",
          position: "Senior SEO Specialist",
          content:
            "5+ years of experience in SEO and content creation. Proficient in keyword research and on-page optimization",
        },
        {
          image: "/images/Picture-3.png",
          name: "Emily Johnson",
          position: "PCC Manager",
          content:
            "3+ years of experience in paid search advertising. Skilled in campaign management and performance analysis",
        },
        {
          image: "/images/Picture-4.png",
          name: "Brian Williams",
          position: "Social Media Specialist",
          content:
            "4+ years of experience in social media marketing. Proficient in creating and scheduling content, analyzing metrics, and building engagement",
        },
        {
          image: "/images/Picture-5.png",
          name: "Sarah Kim",
          position: "Content Creator",
          content:
            "2+ years of experience in writing and editing Skilled in creating compelling, SEO-optimized content for various industries",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="flex flex-col gap-y-10 mb-10">
    <div class="mt-14 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5 xl:gap-10">
      <div class="" v-for="(item, index) in teams" :key="index">
        <div
          class="border border-[#191A23] border-b-[#191A23] rounded-[45px] shadow-[0px_5px_0px_0px_#191A23] py-10 px-[35px] lg:min-h-[350px]"
        >
          <div class="border-b border-black pb-5 flex gap-x-5">
            <img
              :src="item.image"
              alt="team_image"
              class="w-[105.65px] h-[102.82px]"
            />
            <div class="flex flex-col justify-between items-end">
              <img
                src="/images/green-linkedin.svg"
                alt="linkedin_icon"
                class="w-[34px] h-[34px]"
              />
              <div class="flex flex-col">
                <h3 class="text-lg xl:text-xl font-medium text-black">{{ item.name }}</h3>
                <p class="font-normal text-base xl:text-lg text-black">
                  {{ item.position }}
                </p>
              </div>
            </div>
          </div>
          <div class="pt-5">
            <p class="text-base xl:text-lg font-normal text-black">{{ item.content }}</p>
          </div>
        </div>
      </div>
    </div>
    <div class="flex md:justify-end">
      <button
        class="text-white text-xl font-normal bg-[#191A23] py-5 px-[35px] rounded-[14px] w-full md:w-fit"
      >
        See all team
      </button>
    </div>
  </div>
</template>
