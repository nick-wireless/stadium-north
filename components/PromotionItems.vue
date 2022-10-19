<template>
  <div class=" grid grid-cols-1 md:grid-cols-3 ">
    <div id="Community" class=" minimum-one-third bg-orange-800 ">
      <div class=" h-12 w-full flex justify-center items-center  text-stone-100 shadow-md">
        <icons-community class=" h-6 inline-block "></icons-community>
        <span class=" m-2 font-semibold tracking-widest ">COMMUNITY</span>
      </div>
      <nuxt-layout name="inset-text">
        <div
          class="flex items-center justify-center h-[18vh] text-center font-bold italic leading-8 tracking-widest text-lg text-stone-100 ">
          'Have your say', Membership, Steering Committes
        </div>
      </nuxt-layout>
    </div>
    <div id="Announcements" class=" minimum-one-third bg-orange-400 ">
      <div class=" h-12 w-full flex justify-center items-center  text-stone-100 shadow">
        <icons-announcement class=" h-6 inline-block "></icons-announcement>
        <span class=" m-2 font-semibold tracking-widest ">ANNOUNCEMENTS</span>
      </div>
      <nuxt-layout name="inset-text">   
        <div
          class="flex items-center justify-center h-[18vh] text-center font-bold italic leading-8 tracking-widest text-lg text-stone-100 ">
            News, Polls & Events
        </div>
      </nuxt-layout>
    </div>
    <div id="Process" class=" minimum-one-third bg-orange-700">
      <div class=" h-12 w-full flex justify-center items-center  text-stone-100 shadow">
        <icons-process class=" h-6 inline-block "></icons-process>
        <span class=" m-2 font-semibold tracking-widest ">PROCESS</span>
      </div>
      <nuxt-layout name="inset-text">
      <div class="flex items-center justify-center h-[18vh] text-center font-bold italic leading-8 tracking-widest text-lg text-stone-100">
        Sports 2050, Achievements, Development Roadmap
      </div>
      </nuxt-layout>
    </div>
  </div>
</template>

<style scoped>
.minimum-one-third {
  min-height: calc((100vh - 85px)/ 10 * 3)
}
.background-one {
  @apply bg-orange-800
}
.background-two {
  @apply bg-orange-400 
}
.background-three {
  @apply bg-orange-600
}
</style>