<template>
 <div class="page">
    <Hero />
    <About />
 </div>
</template>

<script>
import About from '@/components/Sections/Tab.vue'
import Hero from '@/components/Sections/Hero.vue'


export default {
  components: {
    About,
    Hero
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
