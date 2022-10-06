<template>
  <div class=" grid grid-cols-1 md:grid-cols-3 ">
    <div id="Community" class=" minimum-one-third background-one ">
      <nuxt-layout name="inset-text">
        <div class=" pt-4 pl-4 font-bold leading-8 tracking-widest text-sm text-stone-100">
          COMMUNITY
        </div>
        <div class=" flex flex-col justify-center items-center text-center font-bold italic leading-8 tracking-widest text-lg text-stone-100 ">
          <div class=" mt-8 ">
            'Have your say', Membership, Steering Committes
          </div>
        </div>
      </nuxt-layout>
    </div>
    <div id="Announcements" class=" minimum-one-third background-two ">
      <nuxt-layout name="inset-text">
        <div class=" pt-4 pl-4 font-bold leading-8 tracking-widest text-sm text-stone-100">
          ANNOUNCEMENTS
        </div>
        <div
          class=" flex flex-col justify-center items-center text-center font-bold italic leading-8 tracking-widest text-lg text-stone-100 ">
          <div class=" mt-8 ">
            News, Polls & Events
          </div>
        </div>
      </nuxt-layout>
    </div>
    <div id="Process" class=" minimum-one-third background-three ">
      <nuxt-layout name="inset-text">
        <div class=" pt-4 pl-4 font-bold leading-8 tracking-widest text-sm text-stone-100">
          PROCESS
        </div>
        <div
          class=" flex flex-col justify-center items-center text-center font-bold italic leading-8 tracking-widest text-lg text-stone-100 ">
          <div class=" mt-8 ">
            Sports 2050, Achievements, Development Roadmap
          </div>
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
  background-color: #0c2450
}
.background-two {
  background-color: #8dc641
}
.background-three {
  background-color: #184179
}
</style>