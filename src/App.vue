<script setup lang="ts">
// import AppButton from "./components/AppButton.vue";
// import AppInput from "./components/AppInput.vue";
// import TheMainNav from "./components/TheMainNav.vue";
// import { useDark } from "@vueuse/core";

// const isDark = useDark();

// import Flexbox from './components/Flexbox.vue'
// import Grid from './components/Grid.vue'
// import Responsive from './components/Responsive.vue'
// import ColorPallete from './components/ColorPallete.vue'
// import Fonts from './components/Fonts.vue'
// import Prose from './components/Prose.vue'
import PricingCard from "./components/PricingCard.vue";
</script>
<template>
  <div class="grid gap-6 p-4 md:grid-cols-2 lg:grid-cols-3 max-w-6xl m-auto">
    <!-- <TheMainNav />
    <form action="">
      <label> </label>
      <AppInput label="Username" />
      <AppButton>Submit</AppButton>
    </form> -->
    <!-- <p class="first-letter:text-5xl selection:bg-blue-500 selection:text-white">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet praesentium minima quis dolores sed tempora, vitae tempore voluptas autem sapiente nemo vel aliquam ad reprehenderit laboriosam consequatur rerum aliquid. Sed nihil veniam magni sequi, qui dignissimos earum vitae unde error officiis libero fuga totam eaque alias placeat a quas atque.
    </p> -->
    <!-- <input type="checkbox" v-model="isDark" /> Dark Mode
    <ul class="list-disc marker:text-2xl marker:text-green-500">
      <li>Vue.js</li>
      <li>React</li>
      <li>Svelte</li>
      <li>Solid</li>
    </ul> -->
    <!-- <Flexbox /> -->
    <!-- <Grid /> -->
    <!-- <Responsive /> -->
    <!-- <ColorPallete /> -->
    <!-- <Fonts /> -->
    <!-- <Prose /> -->
    <PricingCard
      :price="29"
      :features="[
        'Unlimited Access to All Features',
        '24/7 Customer Support',
        'Customizable Dashboard',
        'Advanced Analytics Tools',
        'Integration with Third-Party Services',
        'Secure Data Encryption',
      ]"
      name="Starter"
      description="Best option for personal use & for your next project."
    ></PricingCard>
    <PricingCard
      name="Plus"
      :features="[
        'Multi-User Collaboration Tools',
        'Real-Time Data Backup',
        'Mobile App Access',
        'Custom Branding Options',
        'Automated Reporting System',
      ]"
      :price="50"
      description="Great for small teams and anyone looking to scale"
    ></PricingCard>

    <PricingCard
      name="Enterprise"
      :features="[
        'Priority Feature Updates',
        'Extended Data Storage Capacity',
        'Personalized User Experience',
        'In-Depth Training Materials',
        'Dedicated Account Manager',
      ]"
      :price="150"
      description="Best for large scale uses and extended redistribution rights."
    ></PricingCard>
  </div>
</template>
