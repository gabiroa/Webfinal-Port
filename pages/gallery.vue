<script setup>
definePageMeta({
  layout: "landing",
});

const TeamImg1 = "https://wp.globaluniversitysystems.com/ue/wp-content/uploads/sites/9/2021/12/uxuidesign_erina-baftiroska_2800x1200px.png?w=1380&h=776&crop=1";
const TeamImg2 = "https://corsoux.it/wp-content/uploads/2023/05/diventare-ux-designer.jpg";
const TeamImg3 = "https://fiverr-res.cloudinary.com/images/t_main1,q_auto,f_auto,q_auto,f_auto/gigs/118123820/original/7c10800a3697becb9036c8c96d58bf4505c549a2/create-an-incredible-ux-and-ui-for-your-product.png";
const TeamImg4 = "https://www.otis.edu/sites/default/files/styles/primary_news_image/public/UXUI%20hero_0.jpg?itok=dXPocHyd";
const TeamImg5 = "https://media.licdn.com/dms/image/D4D12AQFCAc9opGujrw/article-cover_image-shrink_720_1280/0/1685613726106?e=2147483647&v=beta&t=HfSIZmxen095ZXH3M82GLYmWyfXzZ8VNZ2WOtLueK5s";
const TeamImg6 = "https://richcoward.com/wp-content/uploads/2021/07/UX-Design.jpeg";

const team = [
  {
    name: "Travel App",
    avatar: {
      src: TeamImg1,
      width: 480,
      height: 560,
    },
  },
  {
    name: "Lo-Fi",
    avatar: {
      src: TeamImg2,
      width: 580,
      height: 580,
    },
  },
  {
    name: "Hi-Fi",
    avatar: {
      src: TeamImg3,
      width: 580,
      height: 580,
    },
    
  },
  {
    name: "Group Collab",
    avatar: {
      src: TeamImg4,
      width: 480,
      height: 560,
    },
  },
  {
    name: "Streaming Website",
    avatar: {
      src: TeamImg5,
      width: 580,
      height: 580,
    },
  },
  {
    name: "Mid-Fi",
    avatar: {
      src: TeamImg6,
      width: 580,
      height: 580,
    },
    
  },
  
];
</script>

<template>
  <LandingContainer>
    <LandingSectionhead>
      <template v-slot:title>Gallery</template>
      <template v-slot:desc>Some of our latest and greatest work.</template>
    </LandingSectionhead>


    <div class="grid md:grid-cols-3 gap-10 mx-auto max-w-4xl mt-12">
      <div v-for="item of team" class="group">
        <div class="w-full aspect-square">
          <img
            :src="item.avatar.src"
            :width="item.avatar.width"
            :height="item.avatar.height"
            format="avif"
            alt="Team"
            class="w-full h-full object-cover rounded transition group-hover:-translate-y-1 group-hover:shadow-xl"
          />
        </div>

        <div class="mt-4 text-center">
          <h2 class="text-lg text-gray-800">{{ item.name }}</h2>
          <h3 class="text-sm text-slate-500">{{ item.title }}</h3>
        </div>
      </div>
      <!-- {
        team.map((item) => (
          <div class="group">
            <div class="w-full aspect-square">
              <Image
                {...item.avatar}
                format="avif"
                alt="Team"
                class="w-full h-full object-cover rounded transition  group-hover:-translate-y-1 group-hover:shadow-xl"
              />
            </div>

            <div class="mt-4 text-center">
              <h2 class="text-lg text-gray-800"> {item.name}</h2>
              <h3 class="text-sm text-slate-500"> {item.title}</h3>
            </div>
          </div>
        ))
      } -->
    </div>
  </LandingContainer>
</template>