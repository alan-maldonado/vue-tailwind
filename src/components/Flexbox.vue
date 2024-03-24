<template>
  <section class="flex flex-wrap items-end justify-center gap-2">
    <div
      v-for="i in 15"
      :key="i"
      class="h-14 w-14 flex-shrink-0 bg-gray-500 p-4 text-center text-white"
      :style="`height: ${i * 30 + 30}px`"
    >
      {{ i }}
    </div>
  </section>
</template>
