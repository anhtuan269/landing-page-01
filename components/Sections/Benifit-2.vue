<template>
  <div class="py-25 bg-white">
      <div
      class="max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl mx-auto py-20 text-center"
    >
        <Heading 
            :title="title"
            :time="time"
            :titl="titl"
            :description="description"
            :tim="tim"
            :show="show"
        />
        <Card :cards="cards" />
       <div class="mt-20 max-w-lg mx-auto">
            <Tes />
       </div>
    </div>
  </div>
</template>

<script>
import Card from '@/components/Card/Card-Icon-Style-2.vue'
import Heading from '@/components/Header/Heading.vue'
import Tes from '@/components/Testimonial/Testimonial-Style-1.vue'
export default {
    data(){
        return {
            description:'',
            title:"Double You",
            titl:"Double You",
            time:'conversion.',
            tim: "growth.",
            show:true,
            cards:[
                {
                    id:1,
                    header:"Brands",
                    icon:'/images/icon-brand.png',
                    title:"Icreases conversions",
                    description:'Enhance the visual showcase of your products with unique content making visitors convert to buyers.'

                },
                {
                    id:2,
                    header:"Maketers",
                    icon:'/images/clock.png',
                    title:"Save times",
                    description:'No more re-purposing, re-cropping or re-uploading the same content from your Instagram stories to your website. '

                },
                {
                    id:3,
                    header:"Fresh content",
                    icon:'/images/time.png',
                    title:"Icreases conversions",
                    description:'Every story you post on Instagram, it is automatically saved in your account. Auto updates you unique content.'

                },
            ]
        }
    },
 components: {
     Heading,
     Card,
     Tes
 }
}
</script>

<style>

</style>