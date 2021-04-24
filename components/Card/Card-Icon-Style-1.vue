<template>
  <div class="flex justify-center items-center ">
    <div class="card bg-white py-8 px-10 mx-2 rounded-xl shadow-xl" v-for="(card, index) in cards" :key="index">
      <img :src="card.source" alt="" class="mx-auto" />
      <h3 class="mt-4 font-semibold text-xl">{{ card.title }}</h3>
      <p class="text-xl font-normal ">{{ card.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    cards: {
      type: Array,
      require: true,
      
    },
    istrue:false
  },
};
</script>

<style>
</style>