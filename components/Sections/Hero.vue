<template>
  <div class="bg-gray-200 ">
    <Header />
    <div
      class="max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl mx-auto py-14"
    >
      <div class="flex justify-between items-center">
        <div class="block">
          <Heading />
          <CTA />
        </div>
        <div class="w-full relative -right-28">
            <img src="@/static/images/hero-banner.png" class="relative -right-2" alt="">
        </div>
      </div>
    <Customer />
    </div>
  </div>
</template>

<script>
import CTA from "@/components/CTA/CTA.vue";
import Customer from'@/components/Customer/Customer.vue';
import Header from "@/components/Header/Header.vue";
import Heading from "@/components/Header/Heading.vue";
export default {
  components: {
    CTA,
    Customer,
    Header,
    Heading,
  },
};
</script>

<style>
</style>