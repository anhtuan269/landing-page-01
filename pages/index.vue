<template>
 <div class="page">
    <Hero />
    <About />
    <Benifit />
    <Benifit_2 />
    <Template />
    <Feature />
    <Feature_2 />
    <Intergration />
    <CTA />
    <Group />
 </div>
</template>

<script>
import About from '@/components/Sections/Tab.vue'
import Benifit from '@/components/Sections/Benifit.vue'
import Benifit_2 from '@/components/Sections/Benifit-2.vue'
import CTA from '@/components/Sections/CTA.vue'
import Feature from '@/components/Sections/Feature.vue'
import Feature_2 from '@/components/Sections/Feature_2.vue'
import Group from '@/components/Sections/Group.vue'
import Hero from '@/components/Sections/Hero.vue'
import Intergration from '@/components/Sections/Intergrations.vue'
import Template from '@/components/Sections/Template.vue'


export default {
  components: {
    About,
    Benifit,
    Benifit_2,
    CTA,
    Feature,
    Feature_2,
    Group,
    Hero,
    Intergration,
    Template
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}


</style>
