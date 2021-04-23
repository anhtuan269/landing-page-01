<template>
 <div class="page">
    <Hero />
 </div>
</template>

<script>
import Hero from '@/components/Sections/Hero.vue'

export default {
  components: {
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
