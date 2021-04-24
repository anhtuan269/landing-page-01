<template>
  <div class="bg-white py-18">
    <div
      class="max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl mx-auto py-20 text-center"
    >
      <img class="mx-auto" src="@/static/images/btn-primary.png" alt="" />
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
        <div class="flex items-center justify-center p-2 mr-3 cursor-pointer ">
          <div class="mr-3">
            <img src="@/static/images/check.png" alt="" />
          </div>
          <p class="text-lg">Simple instalation. No developers needed</p>
        </div>
         <div class="flex items-center justify-center p-2 mr-3 cursor-pointer ">
          <div class="mr-3">
            <img src="@/static/images/check.png" alt="" />
          </div>
          <p class="text-lg">Embed on different CMS platforms</p>
        </div>
         <div class="flex items-center justify-center p-2 mr-3 cursor-pointer ">
          <div class="mr-3">
            <img src="@/static/images/check.png" alt="" />
          </div>
          <p class="text-lg">Auto sync new stories</p>
        </div>
      </div>
      <div class="relative">
        <img src="@/static/4.png" alt="" />
      </div>
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
      title: "Embed it and forget it",
      titl: "",
      title_second: "",
      description: " ",
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