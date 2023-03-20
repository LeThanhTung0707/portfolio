<template>
  <div id="navbar" class="flex justify-center backdrop-blur-xl fixed w-full z-50 duration-1000">
    <div class="flex flex-row justify-between items-center w-full max-w-[1344px] relative">
      <div class="animate__fadeInDown animate__animated delay1">
        <img class="h-[80px]" src="/images/logo.png" alt="">
      </div>
      <div class="px-10 h-full flex justify-center items-center md:hidden" @click="() => {hiddenMenu = !hiddenMenu}"><i class="ri-menu-line"></i></div>
      <div :class="hiddenMenu ? 'hidden' : 'flex'" class=" bg-white backdrop-blur-sm md:bg-transparent md:flex absolute top-[100%] w-full md:relative md:top-0 justify-center items-center md:justify-end  flex-col md:flex-row md:space-x-10 md:px-10 text-[18px]">
        <NuxtLink to="#about">
          <div @click="() => {hiddenMenu = !hiddenMenu}" class="animate__fadeInDown animate__animated delay2 cursor-pointer hover:text-rose-900">About</div>
        </NuxtLink>
        <NuxtLink to="#experience">
          <div @click="() => {hiddenMenu = !hiddenMenu}" class="animate__fadeInDown animate__animated delay3 cursor-pointer hover:text-rose-900">Experience</div>
        </NuxtLink>
        <NuxtLink to="#work">
          <div @click="() => {hiddenMenu = !hiddenMenu}" class="animate__fadeInDown animate__animated delay4 cursor-pointer hover:text-rose-900">Work</div>
        </NuxtLink>
        <NuxtLink to="#contact">
          <div @click="() => {hiddenMenu = !hiddenMenu}" class="animate__fadeInDown animate__animated delay5 cursor-pointer hover:text-rose-900">Contact</div>
        </NuxtLink>
      </div>
    </div>
  </div>
  <div>
    <slot />
  </div>
  <div class="mix-blend-difference animate__fadeIn animate__animated delay5 hidden md:flex fixed bottom-0 left-0 items-end ml-7 text-rose-800">
    <div class="flex flex-col ">
      <a href="https://www.facebook.com/tung.lethanh.3532507/" target="_blank">
        <div class="text-[20px]"><i class="ri-facebook-line"></i></div>
      </a>
      <a href="https://www.instagram.com/le_ethanhtung_f/" target="_blank">
        <div class="text-[20px]"><i class="ri-instagram-line"></i></div>
      </a>
      <div class="w-[1px] h-[90px] bg-rose-800 m-auto"></div>
    </div>
  </div>
  <div orientation="right" class="mix-blend-difference animate__fadeIn animate__animated delay5 hidden md:flex fixed bottom-0 right-0 items-end mr-3 text-rose-800">
    <div class="flex flex-col">
      <div class="write mb-3">tenanhlavip@gmail.com </div>
      <div class="w-[1px] h-[90px] bg-rose-800 m-auto"></div>
    </div>
  </div>
</template>

<script setup lang="ts">
const hiddenMenu = ref<boolean>(true)
const lastScrollTop = ref<number>(0)
onMounted(() => {
  addEventListener('scroll' , () => {
    hiddenMenu.value = true;
    const navbar = document.getElementById('navbar')
    const scrollTop = window.pageYOffset || document.documentElement.scrollTop;
    if (scrollTop > lastScrollTop.value) {
      navbar.style.top = '-80px'
    } else {
      navbar.style.top = '0px'
    }
    if( scrollTop != 0 ) {
      navbar.style.borderBottom = '1px'
      navbar.style.boxShadow = "-15px 0px 10px -15px #111"
    } else {
      navbar.style.borderBottom = '0px'
      navbar.style.boxShadow = 'none'
    }
    lastScrollTop.value = scrollTop
  })
})
</script>

<style>
.delay1 {
  animation-delay: 100ms;
}
.delay2 {
  animation-delay: 300ms;
}
.delay3 {
  animation-delay: 500ms;
}
.delay4 {
  animation-delay: 700ms;
}
.delay5 {
  animation-delay: 900ms;
}
.write {
  -webkit-writing-mode: vertical-rl;
  writing-mode: vertical-rl;
}
</style>