<template>
  <div class="mt-20 flex justify-center items-center">
      <div class="card bg-gray-200 text-left p-4 mx-4" v-for="(card, index) in cards" :key="index">
            <h3 class="mb-4 text-3xl font-semibold ">{{card.header}}</h3>
            <div class="flex items-center">
                <div class="block">
                    <img :src="card.icon" alt="">
                </div>
                <h4 class=" text-2xl font-black ml-4">{{card.title}}</h4>
            </div>
            <div class="mt-3">
                {{card.description}}
            </div>
      </div>
  </div>
</template>

<script>
export default {
    props: {
        cards: {
            type: Object
        }
    }

    }
</script>

<style>

</style>