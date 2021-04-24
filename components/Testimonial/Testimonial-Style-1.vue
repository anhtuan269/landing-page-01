<template>
  <div class="text-center">
      <img :src="img" alt="" class="mx-auto mb-4">
      <div class="mt4">
          <p class="text-lg font-normal">{{description}}</p>
      </div>
      <div class="flex justify-center items-center mt-4">
          <div class=" block">
              <img :src="source" alt="">
          </div>
          <h3 class="ml-6">
              <span class="font-bold text-xl">Ben Calahen, </span>
              <span class="text-xl">COO at Clovin</span>
          </h3>
      </div>
  </div>
</template>

<script>
export default {
props: {
    source: {
        type:String,
        default() {
            return '/images/Ben.png'
        }
    },
    img: {
        type:String,
        default() {
            return '/images/testimonial-image.png'
        }
    },
    description:{
        type:String,
        default() {
            return  "“Storytelling on another level. EmbedStories is great - it takes pride of place on our homepage aggregating stories from our Instagram account. I highly recommend this product. ”."
        }
    }
}
}
</script>

<style>

</style>