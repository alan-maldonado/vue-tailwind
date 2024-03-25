<script setup lang="ts">
import CartCheckoutColumnLeft from "./CartCheckoutColumnLeft.vue";
import CartCheckoutColumnRight from "./CartCheckoutColumnRight.vue";
import CartCheckoutShadow from "./CartCheckoutShadow.vue";
</script>
<template>
  <div class="relative">
    <div
      class="relative z-10 grid grid-cols-9 overflow-hidden rounded-2xl border-2 border-white bg-[#323239]"
    >
      <CartCheckoutColumnLeft />
      <CartCheckoutColumnRight />
    </div>
    <CartCheckoutShadow />
  </div>
</template>
