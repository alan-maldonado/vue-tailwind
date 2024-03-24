<script setup lang="ts">
import AppButton from "./components/AppButton.vue";
import AppInput from "./components/AppInput.vue";
import TheMainNav from "./components/TheMainNav.vue";
</script>
<template>
  <div class="m-10">
    <!-- <TheMainNav />
    <form action="">
      <label> </label>
      <AppInput label="Username" />
      <AppButton>Submit</AppButton>
    </form> -->
    <!-- <p class="first-letter:text-5xl selection:bg-blue-500 selection:text-white">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet praesentium minima quis dolores sed tempora, vitae tempore voluptas autem sapiente nemo vel aliquam ad reprehenderit laboriosam consequatur rerum aliquid. Sed nihil veniam magni sequi, qui dignissimos earum vitae unde error officiis libero fuga totam eaque alias placeat a quas atque.
    </p> -->
    <ul class="list-disc marker:text-green-500 marker:text-2xl">
      <li>Vue.js</li>
      <li>React</li>
      <li>Svelte</li>
      <li>Solid</li>
    </ul>
  </div>
</template>