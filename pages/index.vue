<template>
  <div class="flex flex-col justify-center min-h-screen items-center pt-[80px] overflow-hidden">
    <section class="delay-first needAnimate max-w-[1344px] px-6 md:px-[100px] w-full pt-[40px] flex flex-col justify-center items-center">
      <div class="flex flex-col justify-center items-center py-10 mt-10">
        <div class="flex flex-col justify-start items-start">
          <div class="font-bold text-[#080808] text-[24px] md:text-[30px] pl-[4px]">Hi, my name is</div>
          <div class="text-[32px] md:text-[48px] font-bold text-[#141C3A]">Lê Thanh Tùng</div>
          <div class="text-[32px] md:text-[48px] font-bold text-[#141C3A] mb-6">I'm Frontend & Backend Developer</div>
          <div class="mb-6 text-[1.5rem] leadding-[1.5]">I code beautifully simple things, and I love what I do.</div>
        </div>
        <div class="mb-6"><img class="w-[150px] md:w-[210px]" src="/images/avatar.png" alt=""></div>
      </div>
      <div class="needAnimate max-w-[100%] md:max-w-[860px] pt-10">
        <img src="/images/pick3.svg" alt="">
      </div>
    </section>
    <section id="about" class="bg-[#080808] w-full flex flex-col justify-center items-center pt-40 pb-72 px-6 md:px-20 text-white">
      <div class="needAnimate w-full lg:w-[60%] flex items-center justify-center flex-col">
        <div class="font-bold text-[24px] md:text-[35px] mb-10 text-center md:text-start">Hi, I’m Tùng. Nice to meet you.</div>
        <h2 style="word-break: break-word;" class="break-words leading-6  md:px-8 text-center mb-10">I’m a software engineer specializing in building exceptional digital experiences. I enjoy creating things that live on the internet. My interest in web development started back in 2022 when I took a course on website design. 
          I'm quietly confident, naturally curious, and perpetually working on improving my chops one develop problem at a time.
        </h2>
      </div>
    </section>
    <section id="experience" class="needAnimate w-full flex flex-col justify-center items-center mt-[-18rem] mb-12 px-2 lg:px-0">
      <div class="max-w-[1000px] grid grid-cols-1 md:grid-cols-2 w-full rounded-3xl overflow-hidden border-[1px] shadow-lg">
        <div class=" bg-white w-full flex flex-col items-center justify-start md:border-r-[1px]">
          <div class="my-20 flex flex-col items-center justify-start">
            <div class="flex items-center justify-center pt-10 pb-4 mt-8">
              <div class="text-white rounded-[50%] bg-[#080808] w-[80px] h-[80px] flex justify-center items-center text-[50px]"><i class="ri-computer-line"></i></div>
            </div>
            <div class="font-bold pb-5 text-[24px]">
              Frontend Developer
            </div>
            <div class="text-center px-10 h-20">Builds the front-end portion of websites and web applications—the part users see and interact with.</div>
            <div class="pt-7 pb-4 text-[20px] text-[#080808] font-bold">Skill</div>
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

        <div class=" bg-white w-full flex flex-col items-center justify-start border-t-[1px] md:border-none">
          <div class="my-20 flex flex-col items-center justify-start">
            <div class="flex items-center justify-center pt-10 pb-4 mt-8">
              <div class="text-white rounded-[50%] bg-[#080808] w-[80px] h-[80px] flex justify-center items-center text-[50px]"><i class="ri-server-line"></i></div>
            </div>
            <div class="font-bold pb-5 text-[24px]">
              Backend Developer
            </div>
            <div class="text-center px-10 h-20">Creates code that does relational mapping to retrieve data from a database</div>
            <div class="pt-7 pb-4 text-[18px] text-[#080808] font-bold">Skill</div>
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
    <section id="work" class="needAnimate w-full flex justify-center items-center flex-col pb-10">
      <div class="flex flex-col justify-center items-center max-w-[1344px] w-full">
        <div class="flex items-center"><span class="mr-6 font-bold text-[24px] md:text-[35px]">Where I've worked</span><h2 class="md:w-[300px] h-[1px] bg-black"></h2></div>
        <div class="flex flex-col md:flex-row w-full md:w-[70%] py-20 space-x-4">
          <div class="h-full flex flex-row md:flex-col">
            <template v-for="(j, ind) in job">
              <div @click="chooseJob(ind)" :class="ind == currentJob ? 'bg-sky-100 cursor-default border-l-[#080808]' : 'hover:bg-sky-200 cursor-pointer'" class="border-l-2 p-3 px-10 w-full duration-1000">{{ j.name }}</div>
            </template>
          </div>
          <div class="h-full mt-4 md:mt-0">
            <div class="flex flex-col h-full ">
              <div class="font-bold text-[20px] leading-[1.3] mb-2 flex flex-col lg:flex-row">{{ desJob.role }}  <span class="text-[#080808] lg:ml-2">@ {{ desJob.name }}</span></div>
              <div class="text-[14px] leading-[1.3] mb-2 opacity-60 font-bold">{{ desJob.duration }}</div>
              <ul class="pt-5">
                <template v-for="d in desJob.description">
                  <li class="py-2 pr-4 lg:pr-0"><span><i class="ri-play-line text-[#080808]"></i></span> {{ d }}</li>
                </template>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>
    
    <section id="contact" class="needAnimate w-full flex justify-center items-center flex-col pb-10 ">
      <div class="font-bold text-[20px]">What's next ?</div>
      <div class="font-bold text-[36px] pb-3">Get In Touch</div>
      <div class="pb-10 text-center lg:text-start">Interested in working together? We should queue up a time to chat. I'll buy the coffee.</div>
      <a href="mailto:lethanhtung12a1la18@gmail.com?subject=Hello&body=Hello!" class="flex items-center justify-center py-2 px-3 rounded-3xl border-[2px] border-green-500 hover:bg-green-500 hover:text-white cursor-pointer duration-500"><i class="ri-links-line px-1"></i>Let's do this</a>
    </section>
    <section class="py-12 bg-[#080808] w-full flex flex-col justify-center items-center">
      <div class="max-w-[1344px] flex flex-col justify-center items-center">
        <div class=" pb-10 flex flex-col w-full items-center">
          <div class="needAnimate col-span-2  flex flex-col text-white pb-10">
            <div class="text-white text-[30px] mb-4">Contact Infomation</div>
            <div><i class="ri-map-pin-2-fill"></i> <span class="font-bold">Address</span> Ho Chi Minh City, Viet Nam</div>
            <div><i class="ri-phone-fill"></i> <span class="font-bold">Phone</span> +84355780316</div>
            <div><i class="ri-mail-fill"></i> <span class="font-bold">Mail</span> lethanhtung12a1la18@gmail.com</div>
            <div class="flex items-center space-x-4 mt-10">
              <a href="https://www.facebook.com/tung.lethanh.3532507/" target="_blank">
                <div class="hover:scale-110"><img class="w-14 h-14" title="FACEBOOK" src="/images/contact/facebook.svg" alt=""></div>
              </a>
              <a href="https://www.instagram.com/le_ethanhtung_f/" target="_blank">
                <div class="hover:scale-110"><img class="w-14 h-14" title="INSTAGRAM" src="/images/contact/instagram.svg" alt=""></div>
              </a>
            </div>
          </div>
          <div class="needAnimate w-full text-white font-bold text-center text-[24px] px-2 md:px-0">Living, learning, & leveling up one day at a time.</div>
        </div>
      </div>
      
    </section>
  </div>
</template>

<script setup lang="ts">
const job = [
  {
    name: 'Pansoft',
    duration: "July 2022 - Present",
    role: "Frontend & Backend Developer",
    description: [
      'Write modern, performant, maintainable code for a diverse array of client projects',
      'Work with a variety of different languages, platforms, frameworks, and content management systems such as JavaScript, TypeScript, Nuxtjs, Nestjs',
      'Write APIs to connect between systems and serve data exchange with frontend'
    ]
  },
  {
    name: 'Stech',
    duration: "February 2022 - June 2022",
    role: "Backend Developer",
    description: [
      'Developed and maintained code for in-house websites primarily using Javascript, TypeScript.',
      'Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness.',
      "Participate in website development (create and update API)",
    ]
  }
]
const currentJob = ref<number>(0)
const desJob = computed(() => {
  return job[currentJob.value]
})
const chooseJob = (ind:number) => {
  if (currentJob.value != ind) currentJob.value = ind;
}


onMounted(() => {
  const section = document.querySelectorAll(".needAnimate");
  const observer = new IntersectionObserver(entries =>  {
    entries.forEach( entry => {
      entry.target.classList.toggle('backIn', entry.isIntersecting)
    })
  })
  section.forEach(sec => observer.observe(sec))
})
</script>

<style>
.backIn {
  -webkit-animation-name: fadeIn;
  animation-name: fadeIn;
  -webkit-animation-duration: 0.3s;
  animation-duration: 0.3s;
  -webkit-animation-duration: var(--animate-duration);
  animation-duration: var(--animate-duration);
  -webkit-animation-fill-mode: both;
  animation-fill-mode: both;
}
.delay-first {
  animation-delay: 500ms;
}
.needAnimate {
  overflow: hidden;
}
</style>