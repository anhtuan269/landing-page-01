<template>
  <div class="block">
      <h2 class="font-black text-5xl leading-60 mb-6 ">
          {{title}}
          <span v-show="spanShow" class="bg-yellow-300 pl-3 pt-2">{{time}}</span>
      </h2>
      <h2  class="font-black text-5xl leading-60 relative -top-8 "> {{title_second}}</h2>
     <div class="block relative -top-2" v-show="show" >
          <h2 class="font-black text-5xl leading-60 ">
          {{titl}}
          <span class="bg-yellow-300 pl-3 pt-2 ">{{tim}}</span>
      </h2>
     </div>
      <p class="text-lg leading-6 font-normal ">{{description}}</p>
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
         titl: {
            type:String,
            default: () => {
                return null
            }
        },
        title_second: {
            type:String,
            default: () => {
                return null
            }
        },
        tim: {
            type: String,
            require: true,
            default: () => {
                return null
            }
        },
        description : {
            type: String,
            require: true,
            default() {
                return "Display Instagram Stories Widget on your website, that auto-syncs, and updates each time you add a photo in your active story. "
            }
        },
        show: {
            type:Boolean,
            default() {
                return false
            }
        },
        spanShow: {
            type:Boolean,
            default() {
                return true
            }
        }

    }
}
</script>

<style>

</style>