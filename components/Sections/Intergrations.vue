<template>
  <div
    class="max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl mx-auto py-20 text-center bg-gray-200 mb-20"
  >
    <div class="flex items-center justify-between px-14">
      <div class="text-left max-w-md">
        <img class="mb-6" src="@/static/images/btn-primary-2.png" alt="" />
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
        <div class="check text-left mt-6">
          <div class="flex items-center justify-start p-2 mr-3 cursor-pointer">
            <div class="mr-3">
              <img src="@/static/images/check.png" alt="" />
            </div>
            <p class="text-lg">Simple instalation. No developers needed</p>
          </div>
          <div class="flex items-center justify-start p-2 mr-3 cursor-pointer">
            <div class="mr-3">
              <img src="@/static/images/check.png" alt="" />
            </div>
            <p class="text-lg">Embed on different CMS platforms</p>
          </div>
        </div>
      </div>
      <div class="image">
        <img src="@/static/images/chart.png" alt="" />
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
      title: "Works with 99.9% of web platforms",
      titl: "",
      title_second: "",
      description:
        "We integrate with tons of other apps, ecoomerce platforms or web builders. Native apps are avaialble, too.  ",
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