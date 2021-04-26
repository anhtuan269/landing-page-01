<template>
  <div
    class="flex justify-between my-40 max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl mx-auto"
  >
    <div class="w-full">
      <TabA v-show="activeTab === 'TabA'" />
      <TabB v-show="activeTab === 'TabB'" />
      <TabC v-show="activeTab === 'TabC'" />
      <TabD v-show="activeTab === 'TabD'" />
      <TabE v-show="activeTab === 'TabE'" />
    </div>
    <div class="text-left ml-6">
      <h2 class="text-5xl heading-70 mb-4 font-black">
        Widgets for every website.
      </h2>
      <ul class="text-left">
        <li
          @click="activeTab = 'TabA'"
          class="mb-6 group flex justify-start items-center cursor-pointer hover:text-blue-600"
        >
          <svg
            width="40"
            height="40"
            viewBox="0 0 40 40"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="relative opacity-1 hover:opacity-0"
            @click="change"
          >
            <rect width="40" height="40" rx="8" :fill="color" />
            <rect
              x="2.99805"
              y="16"
              width="10"
              height="10"
              rx="5"
              fill="#F9FAFD"
            />
            <rect
              x="14.998"
              y="16"
              width="10"
              height="10"
              rx="5"
              fill="#F9FAFD"
            />
            <rect
              x="26.998"
              y="16"
              width="10"
              height="10"
              rx="5"
              fill="#F9FAFD"
            />
          </svg>
          <svg
            width="40"
            height="40"
            viewBox="0 0 40 40"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="absolute opacity-0 hover:opacity-1"
          >
            <rect width="40" height="40" rx="8" fill="#0066ff" />
            <rect
              x="2.99805"
              y="16"
              width="10"
              height="10"
              rx="5"
              fill="#F9FAFD"
            />
            <rect
              x="14.998"
              y="16"
              width="10"
              height="10"
              rx="5"
              fill="#F9FAFD"
            />
            <rect
              x="26.998"
              y="16"
              width="10"
              height="10"
              rx="5"
              fill="#F9FAFD"
            />
          </svg>

          <p
            class="group-focus: ml-4 text-xl hover:text-blue-600 duration-500 ease-linear"
          >
            Hightlight
          </p>
        </li>
        <li
          @click="activeTab = 'TabB'"
          class="mb-6 group flex hover:text-blue-600 justify-start items-center cursor-pointer"
        >
          <img src="@/static/images/tab-2.png" alt="" />
          <p
            class="group-focus: ml-4 text-xl hover:text-blue-600 duration-500 ease-linear"
          >
            Popover
          </p>
        </li>
        <li
          @click="activeTab = 'TabC'"
          class="mb-6 group flex hover:text-blue-600 justify-start items-center cursor-pointer"
        >
          <img src="@/static/images/tab-3.png" alt="" />
          <p
            class="group-focus: ml-4 text-xl hover:text-blue-600 duration-500 ease-linear"
          >
            Inline slideshows
          </p>
        </li>
        <li
          @click="activeTab = 'TabD'"
          class="mb-6 group flex hover:text-blue-600 justify-start items-center cursor-pointer"
        >
          <img src="@/static/images/tab-4.png" alt="" />
          <p
            class="group-focus: ml-4 text-xl hover:text-blue-600 duration-500 ease-linear"
          >
            Story list gallery
          </p>
        </li>
        <li
          @click="activeTab = 'TabE'"
          class="flex group hover:text-blue-600 justify-start items-center cursor-pointer active-menu"
        >
          <img src="@/static/images/tab-5.png" alt="" />
          <p class="group-focus: ml-4 text-xl">
            Carousel gallery
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import TabA from "@/components/Tab/TabA.vue";
import TabB from "@/components/Tab/TabB.vue";
import TabC from "@/components/Tab/TabC.vue";
import TabD from "@/components/Tab/TabD.vue";
import TabE from "@/components/Tab/TabE.vue";
export default {
  name:'TAb',
  components: {
    TabA,
    TabB,
    TabC,
    TabD,
    TabE,
  },
  data() {
    return {
      activeTab: "TabA",
      color:' #9CA0AC'
    };
  },
  methods: {
      change() {
          console.log(1)
          return this.color = "#0066ff"
      }
  }
};
</script>

<style>
.active-menu {
  @apply text-red-600
    ;
}
</style>