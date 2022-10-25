<template>
  <nuxt-layout name="section-copy" class=" pb-16 ">
    <template #header> 
      <nuxt-layout name="section-heading" >
        <template #subHeading>A stage for the Territory</template>
        <template #default>Imagining what a Stadium could mean for Territorians present, past and future</template>
      </nuxt-layout>
    </template>
    <template #default>
      <div class=" flex flex-wrap ">
        <p class=" xs:max-w-[320px] sm:pr-4 sm:mr-16  "> 
          A home stadium for AFL Australia’s 20th team can become a place for all of the Territory to shine. Athletes, join the
          field to contest the ball; spectators lean back to revel in local competition bested by visiting teams from across
          Australia and the youth bound with excitement for a new vision to tomorrow and what it may behold.
        </p>
        <p class=" xs:max-w-[320px] mt-6 xs:mt-1"> 
          The Northern Territory steps up. Steps up side by side with the support of communities through northern Australia, led
          by Larrakia peoples the land of the City. Stepping up with roots tied deeply to our land the extended into Australia’s
          country like no other. We are ready. Ready to welcome you on Larrakia land.
        </p> 
      </div>
    </template>
    <template #footer>
      <p class=" italic text-teal-700 ">Join your support for our mission here</p>
      <button class="block xs:inline-block ">
        <div class=" flex items-center py-1 px-1 flex-none rounded border-2 border-slate-400 text-gray-700  hover:text-white hover:bg-slate-400 ">
          <span class=" pl-2 font-normal tracking-wider ">Membership signup</span>
          <icons-right class=" h-7 w-7 "></icons-right>
        </div>
      </button>
      <button class=" block xs:inline-block mt-6 w-[204px] mx-6 ">
        <div
          class=" flex items-center py-1 px-1 flex-none rounded border-slate-400 text-gray-700  hover:text-white hover:bg-slate-400 ">
          <span class=" pl-2 font-normal tracking-wider ">Newsletter signup</span>
          <icons-right class=" h-7 w-7 "></icons-right>
        </div>
      </button>
    </template>
  </nuxt-layout>
</template>