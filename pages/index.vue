<template>
  <div class="flex flex-col justify-center min-h-screen items-center pt-[80px]">
    <section class="max-w-[1344px] px-[100px] w-full pt-[40px] flex flex-col justify-center items-center">
      <div class="flex flex-col justify-center items-center py-10 mt-10">
        <div class="flex flex-col justify-start items-start">
          <div class="font-bold text-[#79ACD9] text-[30px] pl-[4px]">Hi, my name is</div>
          <div class="text-[48px] font-bold text-[#141C3A]">Lê Thanh Tùng</div>
          <div class="text-[48px] font-bold text-[#141C3A] mb-6">I'm Frontend & Backend Developer</div>
          <div class="mb-6 text-[1.5rem] leadding-[1.5]">I code beautifully simple things, and I love what I do.</div>
        </div>
        <div class="mb-6"><img class="w-[150px] md:w-[210px]" src="/images/avatar.png" alt=""></div>
      </div>
      <div class="max-w-[100%] md:max-w-[860px] pt-10">
        <img src="/images/pick3.svg" alt="">
      </div>
    </section>
    <section class="bg-[#79ACD9] w-full flex flex-col justify-center items-center pt-40 pb-72 px-20 text-white">
      <div class="w-[60%] flex items-center justify-center flex-col">
        <div class="font-bold text-[35px] mb-10">Hi, I’m Tùng. Nice to meet you.</div>
        <h2 style="word-break: break-word;" class="break-words leading-6  px-8 text-center mb-10">I’m a software engineer specializing in building exceptional digital experiences. I enjoy creating things that live on the internet. My interest in web development started back in 2022 when I took a course on website design. 
          I'm quietly confident, naturally curious, and perpetually working on improving my chops one develop problem at a time.
        </h2>
      </div>
    </section>
    <section class="w-full flex flex-col justify-center items-center mt-[-18rem] mb-12">
      <div class="max-w-[1000px] grid grid-cols-2 w-full rounded-3xl overflow-hidden border-[1px]">
        <div class=" bg-white w-full flex flex-col items-center justify-start border-r-[1px]">
          <div class="my-20 flex flex-col items-center justify-start">
            <div class="flex items-center justify-center pt-10 pb-4 mt-8">
              <div class="text-white rounded-[50%] bg-[#79ACD9] w-[80px] h-[80px] flex justify-center items-center text-[50px]"><i class="ri-computer-line"></i></div>
            </div>
            <div class="font-bold pb-5 text-[24px]">
              Frontend Developer
            </div>
            <div class="text-center px-10 h-20">Builds the front-end portion of websites and web applications—the part users see and interact with.</div>
            <div class="pt-7 pb-4 text-[20px] text-[#79ACD9]">Skill</div>
            <div class="grid grid-cols-4 gap-4 mt-8 ">
              <div class="hover:scale-110 w-[64px] h-[64px] text-[64px] flex items-center text-orange-600" title="HTML"><i class="ri-html5-fill"></i></div>
              <div class="hover:scale-110 w-[64px] h-[64px]"><img class="w-[64px] h-[64px]" title="CSS" src="/images/skill/css.svg"></div>
              <div class="hover:scale-110 w-[64px] h-[64px]"><img class="w-[64px] h-[64px]" title="Javascript" src="/images/skill/javascript.svg" alt=""></div>
              <div class="hover:scale-110 w-[64px] h-[64px]"><img class="w-[64px] h-[64px]" title="Vuejs" src="/images/skill/vuejs.svg" alt=""></div>
              <div class="hover:scale-110 w-[64px] h-[64px]"><img title="NuxtJs" src="/images/skill/nuxt.svg"></div>
              <div class="hover:scale-110 w-[64px] h-[64px]"><img title="Tailwindcss" src="/images/skill/tailwindcss.svg"></div>
            </div>
          </div>
        </div>

        <div class=" bg-white w-full flex flex-col items-center justify-start">
          <div class="my-20 flex flex-col items-center justify-start">
            <div class="flex items-center justify-center pt-10 pb-4 mt-8">
              <div class="text-white rounded-[50%] bg-[#79ACD9] w-[80px] h-[80px] flex justify-center items-center text-[50px]"><i class="ri-server-line"></i></div>
            </div>
            <div class="font-bold pb-5 text-[24px]">
              Backend Developer
            </div>
            <div class="text-center px-10 h-20">Creates code that does relational mapping to retrieve data from a database</div>
            <div class="pt-7 pb-4 text-[18px] text-[#79ACD9] font-bold">Skill</div>
            <div class="grid grid-cols-4 gap-4 mt-8 ">
              <div class="hover:scale-110"><img title="Nodejs" src="/images/skill/nodejs-icon.svg" alt=""></div>
              <div class="hover:scale-110 "><img title="Expressjs" src="/images/skill/expressjs.svg" alt=""></div>
              <div class="hover:scale-110 "><img title="Nestjs" src="/images/skill/nestjs.svg" alt=""></div>
              <div class="hover:scale-110 "><img title="Mongodb" src="/images/skill/mongodb.svg" alt=""></div>
              <div class="hover:scale-110 "><img title="Redis" src="/images/skill/redis.svg" alt=""></div>
              <div class="hover:scale-110 "><img title="Socketio" src="/images/skill/socketio.svg" alt=""></div>
              <div class="hover:scale-110 w-16 h-16"><img title="MikroORM" src="/images/skill/mikroorm.png" alt=""></div>
              <div class="hover:scale-110 "><img title="Neo4j" src="/images/skill/neo4j.svg" alt=""></div>
            </div>
          </div>
        </div>

      </div>
    </section>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>

</style>