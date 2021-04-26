<template>
  <div class="bg-gray-200 mb-20 ">
    <div
      class="max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-2xl mx-auto py-20 text-center"
    >
      <div class="flex items-center justify-between">
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
          <div class="mt-6">
              <CTA />
          </div>
        </div>
        <div class="img">
            <img src="@/static/images/CTA.png" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Heading from "@/components/Header/Heading.vue";
import CTA from '@/components/CTA/CTA.vue'
export default {
  components: {
    Heading,
    CTA
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