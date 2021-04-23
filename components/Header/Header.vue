<template>
 <div class="bg-white">
    <div
    class="max-w-screen-sm md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl mx-auto py-3"
  >
    <div class="flex justify-between items-center">
      <div class="flex items-center">
        <img src="@/static/images/black-logo.png" alt="" />
        <h5 class="ml-2.5 text-lg font-bold leading-tight">embedsocial</h5>
      </div>
      <div class="menu">
        <ul class="flex items-center justify-center">
          <li
            class="py-3 cursor-pointer hover:text-blue-500 duration-500 ease-linear mr-7"
          >
            Playform
            <fa icon="angle-down" />
          </li>
          <li class="py-3 cursor-pointer hover:text-blue-500 duration-500 ease-linear mr-7">Widgets</li>
          <li class="py-3 cursor-pointer hover:text-blue-500 duration-500 ease-linear  mr-7">Templates</li>
          <li class="py-3 cursor-pointer hover:text-blue-500 duration-500 ease-linear ">Pricing</li>
        </ul>
      </div>
      <div class="flex justify-center items-center">
        <p class="cusor-pointer hover:text-blue-500 duration-500 ease-linear mr-7 cursor-pointer"> Login</p>
        <button class="text-white bg-blue-500 p-4 font-bold rounded-md cursor-pointer hover:bg-blue-400 duration-500 ease-linear"> Start Free Trial</button>
      </div>
    </div>
  </div>
 </div>
</template>

<script>
export default {};
</script>

<style>
</style>