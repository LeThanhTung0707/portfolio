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
      <a href="https://www.hackerrank.com/lethanhtung12a11" target="_blank">
        <div class="w-5 h-5 flex justify-center items-center mb-2"><svg height="20" width="20" xmlns="http://www.w3.org/2000/svg" viewBox="-1 -1 582 486.999"><path d="M-1-1h582v402H-1z" fill="none"/><path d="M454.843 141.001c-13.019-22.417-172.832-115-198.859-115-26.019 0-185.895 92.351-198.84 115-12.947 22.649-13.019 207.358 0 230.009 13.018 22.639 172.839 114.989 198.84 114.989 26 0 185.841-92.466 198.851-114.999 13.007-22.533 13.016-207.583.008-229.999zM309.862 398.15c-3.559 0-36.756-32.137-34.141-34.762.781-.78 5.625-1.328 15.768-1.644 0-23.564.53-61.622.844-77.553.038-1.814-.395-3.081-.395-5.256h-71.812c0 6.379-.412 32.523 1.232 65.479.205 4.078-1.42 5.353-5.158 5.335-9.102-.025-18.211-.099-27.321-.071-3.683.009-5.274-1.374-5.157-5.488.826-30.043 2.66-75.488-.134-191.07v-2.849c-8.688-.314-14.717-.862-15.508-1.652-2.624-2.624 31.032-34.76 34.581-34.76 3.558 0 36.989 32.145 34.383 34.76-.782.781-7.098 1.338-15.067 1.652v2.84c-2.174 23.135-1.823 71.506-2.362 94.686h72.107c0-4.089.351-31.212-1.077-75.145-.091-3.047.853-4.646 3.781-4.672 9.945-.072 19.9-.117 29.855-.055 3.108.019 4.105 1.546 4.043 4.834-3.28 171.861-.594 159.867-.594 188.975 7.97.315 15.112.864 15.895 1.655 2.588 2.615-30.205 34.761-33.763 34.761z" fill="#2ec866"/></svg></div>
      </a>
      <a href="https://www.facebook.com/tung.lethanh.3532507/" target="_blank">
        <div class="text-[20px]"><i class="ri-facebook-line"></i></div>
      </a>
      <a href="https://www.instagram.com/le_ethanhtung_f/" target="_blank">
        <div class="text-[20px]"><i class="ri-instagram-line"></i></div>
      </a>
      <a href="https://www.linkedin.com/in/lethanhtungdev77/" target="_blank">
        <div class="text-[20px]"><i class="ri-linkedin-line"></i></div>
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