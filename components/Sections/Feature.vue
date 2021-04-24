<template>
  <div class="bg-white py-18">
    <div
      class="max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl mx-auto py-20 text-center"
    >
      <img class="mx-auto" src="@/static/images/btn-primary-lg.png" alt="" />
      <div class="mt-4">
        <Heading
          :title="title"
          :time="time"
          :titl="titl"
          :title_second="title_second"
          :description="description"
          :tim="tim"
          :show="show"
          :spanShow="spanShow"
        />
      </div>
      <div class="flex items-center justify-center mt-5 mb-10">
        <div class="flex items-center justify-center bg-gray-200 p-2 mr-3 cursor-pointer">
            <div class="mr-2">
                <img src="@/static/images/stories.png" alt="">
            </div>
            <p>Stories from specific date</p>
        </div>
         <div class="flex items-center justify-center bg-gray-200 p-2 mr-3 cursor-pointer">
            <div class="mr-2">
                <img src="@/static/images/custom.png" alt="">
            </div>
            <p>Customize color</p>
        </div>
         <div class="flex items-center justify-center bg-gray-200 p-2 mr-3 cursor-pointer">
            <div class="mr-2">
                <img src="@/static/images/instag.png" alt="">
            </div>
            <p>Follow button</p>
        </div>
         <div class="flex items-center justify-center bg-gray-200 p-2 mr-3 cursor-pointer">
            <div class="mr-2">
                <img src="@/static/images/multi.png" alt="">
            </div>
            <p>Multiple layouts</p>
        </div>
         <div class="flex items-center justify-center bg-gray-200 p-2 mr-3 cursor-pointer">
            <div class="mr-2">
                <img src="@/static/images/setting.png" alt="">
            </div>
            <p>Advance moderation</p>
        </div>
         <div class="flex items-center justify-center bg-gray-200 p-2 mr-3 cursor-pointer">
            <div class="mr-2">
                <img src="@/static/images/mini-logo.png" alt="">
            </div>
            <p>Custom CSS</p>
        </div>

      </div>
      <img src="@/static/images/feature-image.png" alt="">
    </div>
  </div>
</template>

<script>
import Heading from "@/components/Header/Heading.vue";
export default {
  components: {
    Heading,
  },
  data() {
    return {
      title: "Be on brand. Customize in minutes",
      titl: "",
      title_second: "",
      description:
        "EmbedStories gives you flexibility in managing the display and looks of the Instagram Stories on your website. ",
      time: "",
      tim: "",
      show: false,
      spanShow: false,
    };
  },
};
</script>

<style>
</style>