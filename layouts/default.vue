<template>
  <div class="flex justify-center backdrop-blur-2xl fixed w-full">
    <div class="flex flex-row justify-between items-center w-full max-w-[1344px]">
      <div class="">
        <img class="h-[80px]" src="/images/logo.png" alt="">
      </div>
      <div class="flex space-x-10 px-10 text-[18px]">
        <div class="cursor-pointer hover:text-[#ddda15]">About</div>
        <div class="cursor-pointer hover:text-[#ddda15]">Experience</div>
        <div class="cursor-pointer hover:text-[#ddda15]">Work</div>
        <div class="cursor-pointer hover:text-[#ddda15]">Contact</div>
      </div>
    </div>
  </div>
  <div>
    <slot />
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>

</style>