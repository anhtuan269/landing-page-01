<template>
  <div class="text-left">
      <h2 class="font-black text-5xl leading-60 mb-7">
          {{title}}
          <span class="bg-yellow-300 pl-3 pt-2">{{time}}</span>
      </h2>
      <h2 class="font-dark text-6xl leading-60 mb-7">
          {{titl}}
          <span class="bg-yellow-300 ">{{tim}}</span>
      </h2>
      <p class="text-lg leading-6 font-normal">{{description}}</p>
  </div>
</template>

<script>
export default {
    props: {
        title: {
            type:String,
            default: () => {
                return "Display Instagram Stories on any website,"
            }
        },
        time: {
            type: String,
            require: true,
            default: () => {
                return "in seconds."
            }
        },
        description : {
            type: String,
            require: true,
            default() {
                return "Display Instagram Stories Widget on your website, that auto-syncs, and updates each time you add a photo in your active story. "
            }
        }

    }
}
</script>

<style>

</style>