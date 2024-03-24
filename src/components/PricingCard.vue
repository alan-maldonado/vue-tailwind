<script setup lang="ts">
defineProps<{
  price: number;
  features: string[];
  name: string;
  description: string;
}>();
</script>
<template>
  <div
    class="flex flex-col justify-between rounded-lg border dark:bg-gray-800 p-4 text-center"
  >
    <div>
      <h3 class="mb-4 text-xl font-bold">{{ name }}</h3>
      <p class="mb-4 text-gray-500">
        {{ description }}
      </p>
      <div class="flex items-center justify-center">
        <span class="mr-2 inline-block text-4xl font-bold">${{ price }}</span>
        <span class="text-gray-500">/month</span>
      </div>
      <!-- List -->
      <ul role="list" class="mt-3 text-left">
        <li v-for="feature in features" :key="feature" class="mb-4 flex">
          <!-- Icon -->
          <svg
            class="mr-2 h-5 w-5 text-green-500"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
              clip-rule="evenodd"
            ></path>
          </svg>
          <span>{{ feature }}</span>
        </li>
      </ul>
    </div>
    <a class="block rounded bg-blue-600 px-4 py-2 text-white" href="#">Get started</a>
  </div>
</template>
