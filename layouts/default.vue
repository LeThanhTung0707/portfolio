<template>
  <div class="flex justify-center backdrop-blur-sm fixed w-full">
    <div class="flex flex-row justify-between items-center w-full max-w-[1344px] relative">
      <div class="">
        <img class="h-[80px]" src="/images/logo.png" alt="">
      </div>
      <div class="px-10 h-full flex justify-center items-center md:hidden" @click="() => {hiddenMenu = !hiddenMenu}"><i class="ri-menu-line"></i></div>
      <div :class="hiddenMenu ? 'hidden' : 'flex'" class="bg-white backdrop-blur-sm md:bg-transparent md:flex absolute top-[100%] w-full md:relative md:top-0 justify-center items-center md:justify-end  flex-col md:flex-row md:space-x-10 md:px-10 text-[18px]">
        <NuxtLink to="#about">
          <div @click="() => {hiddenMenu = !hiddenMenu}" class="cursor-pointer hover:text-[#79ACD9]">About</div>
        </NuxtLink>
        <NuxtLink to="#experience">
          <div @click="() => {hiddenMenu = !hiddenMenu}" class="cursor-pointer hover:text-[#79ACD9]">Experience</div>
        </NuxtLink>
        <NuxtLink to="#work">
          <div @click="() => {hiddenMenu = !hiddenMenu}" class="cursor-pointer hover:text-[#79ACD9]">Work</div>
        </NuxtLink>
        <NuxtLink to="#contact">
          <div @click="() => {hiddenMenu = !hiddenMenu}" class="cursor-pointer hover:text-[#79ACD9]">Contact</div>
        </NuxtLink>
      </div>
    </div>
  </div>
  <div>
    <slot />
  </div>
</template>

<script setup lang="ts">
const hiddenMenu = ref<boolean>(true)
onMounted(() => {
  addEventListener('scroll' , () => {
    hiddenMenu.value = true
  })
})
</script>

<style scoped>

</style>