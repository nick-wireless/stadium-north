<template>
  <div class=" flex items-center ">
    <div class=" my-2 p-[4px]  w-10 h-10 text-current drop-shadow-lg ">
      <slot></slot>
    </div>
    <span class=" pl-2 ">{{ iconName }}</span>
  </div>
</template>

<script>
export default {
  props: {
    iconName: String
  }
}
</script>

<style scoped>

</style>