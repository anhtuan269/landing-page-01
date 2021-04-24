<template>
  <div class="bg-black py-20">
    <div
      class="max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl mx-auto py-20 text-center text-white"
    >
      <div class="max-w-xl mx-auto">
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
      <div class="text-center mt-10">
        <div
          class="btn bg-blue-500 p-4 rounded-xl text-white inline-block font-bold hover:bg-blue-600 duration-500 ease-linear cursor-pointer"
        >
          See templates demos
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Heading from "@/components/Header/Heading.vue";
export default {
  data() {
    return {
      title: "Get started with one of our templates",
      titl: "",
      title_second: "",
      description:
        "Start with one of our pre-designed templates. Create, personalize and embed the perfect widget for any page or campaign in just minutes.",
      time: "",
      tim: "",
      show: false,
      spanShow: false,
    };
  },
  components: {
    Heading,
  },
};
</script>

<style>
</style>