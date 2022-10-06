<template>
  <div class=" flex items-center ">
    <div class=" pt-2  w-8 h-8 text-current drop-shadow-lg ">
      <slot></slot>
    </div>
    <span class=" pl-3 pt-4 ">{{ iconName }}</span>
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