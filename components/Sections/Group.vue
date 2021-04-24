<template>
  <div class="bg-gray-200 py-20">
      <div class="max-w-xl mx-auto text-center" >
          <Heading :description="description" :title="title" :titl="titl" :title_second="title_second" :show="show" :time="time" :spanShow="spanShow" />
        <div class="flex justify-center">
              <CTA />
        </div>
      </div>
  </div>
</template>

<script>
import Heading from '@/components/Header/Heading.vue'
import CTA from '@/components/CTA/CTA.vue'
export default {
    components: {
        Heading,
        CTA
    },
    data() {
        return {
            description:'Display Instagram Stories Widget on your website, that auto-syncs, and updates each time you add a photo in your active story. ',
            title:"Ready to dive in?",
            title_second:"Create your widget today.",
            time:null,
            tim: "",
            show:false,
            spanShow: false,
            titl: ''
        }
    }
}
</script>

<style>

</style>