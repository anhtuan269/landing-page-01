<template>
  <div class="bg-gray-200">
    <div
      class="max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl mx-auto py-20 text-center"
    >
      <div class="max-w-3xl mx-auto">
        <Heading :title="title" :time="time" :description="description" />
      </div>
      <div class="mt-18">
          <Card :cards="cards"/>
      </div>
    </div>
  </div>
</template>

<script>
import Card from '@/components/Card/Card-Icon-Style-1.vue'
import Heading from "@/components/Header/Heading.vue";
export default {
  data() {
    return {
      title: "Let your story live",
      time: " more than 24h.",
      description:"You've worked hard to create a beautiful Instagram story but it disappears in 24 hours? No worries, use our story saver for Instagram to bring them to life on your website.",
      cards:  [
          {
            id: 1,
            source: "/images/instagram.png",
            title: "Auto-Sync ",
            description: "Instagram Stories",
          },
          {
            id: 2,
            source: "/images/facebook.png",
            title: "Upload ",
            description: "Facebook Stories",
          },
          {
            id: 3,
            source: "/images/toktok.png",
            title: "Sync ",
            description: "TikTok Stories",
          },
          {
            id: 4,
            source: "/images/twitter.png",
            title: "Upload ",
            description: "Twitter Stories",
          },
          {
            id: 5,
            source: "/images/in.png",
            title: "Auto-Sync ",
            description: "LinkedIn Stories",
          },
      ]
    };
  },
  components: {
      Card,
    Heading
  },
};
</script>

<style>
</style>