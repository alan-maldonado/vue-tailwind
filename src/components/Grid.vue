<template>
  <section class="grid grid-flow-dense grid-cols-4 gap-2">
    <div></div>
    <div></div>
    <div class="flex items-center justify-around col-span-3">
      <div class="w-16 min-h-0 h-16 bg-green-300"></div>
      <div class="w-16 min-h-0 h-16 bg-blue-300"></div>
      <div class="w-16 min-h-0 h-16 bg-green-300"></div>
      <div class="w-16 min-h-0 h-16 bg-blue-300"></div>
    </div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
  </section>
</template>

<style scoped>
div {
  @apply min-h-[100px] bg-gray-400 even:bg-gray-600;
}
</style>
