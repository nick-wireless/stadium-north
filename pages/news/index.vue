<template>
  <the-header></the-header>
  <nuxt-layout name="inset-text">
    <div class=" text-gray-800 pt-8">
      <!-- Title particulars -->
      <h1 class=" pt-12 pb-4 font-bold text-2xl xs:text-3xl leading-9  ">Catherine, Princess of Wales, follows in footsteps of mother-in-law Diana as she takes on a title with baggage</h1>
      <div id="article-details" class=" pb-8 ">
        <span>Updated by {{ teamWriters }}</span>
        <div id="date-line">Posted, {{ datePublished }}</div>
      </div>
      
      <div id="article-hero-image" class="relative overflow-hidden h-[200px] sm:h-[420px] lg:h-[540px] "> 
        <img class=" absolute h-full w-full object-cover object-bottom "
          src="@/assets/images/02alvin-balemesa---kNU__Bb-g-unsplash.jpg"
          alt="" />
      </div>
      <div class=" pt-4 py-10 text-sm text-slate-500 ">{{ pictureFooter }}</div>
      
      <share-with-friends></share-with-friends>

      <p class=" pt-12 pb-16 leading-9 tracking-wide font-work ">
        <slot> {{ copyArticle }} </slot>
      </p>
    </div>
  </nuxt-layout>
  <the-footer></the-footer>
</template>

<script>
export default {
  data() {
    return {
      teamWriters: 'Delivery Team',
      datePublished: 'Sun 21st Aug 2022',
      pictureFooter: 'Image description here, they can be fairly long.',
      copyArticle: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Debitis sapiente dolores, iure quam voluptas minus doloremque, qui nisi quia vel totam tempore odit ratione blanditiis omnis ducimus, expedita sit tempora.'
      }
    }
  }
</script>