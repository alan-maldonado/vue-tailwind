<script setup lang="ts">
import { ref } from "vue";
const active = ref(false);
const mobileMenuActive = ref(true);
// const mobileMenuActive = ref(false);
</script>

<template>
  <header class="relative flex items-center justify-between bg-gray-800 p-2">
    <button
      @click="mobileMenuActive = !mobileMenuActive"
      class="flex w-8 flex-col gap-1 bg-gray-700 p-2 outline outline-white sm:hidden"
    >
      <span class="block h-[2px] w-full bg-white"></span>
      <span class="block h-[2px] w-full bg-white"></span>
      <span class="block h-[2px] w-full bg-white"></span>
    </button>
    <div class="flex items-center">
      <img
        src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=500"
        alt="logo"
        class="h-16 w-16 sm:mr-3"
      />
      <ul
        class="absolute left-0 top-full flex w-full flex-col gap-1 bg-gray-800 p-2 sm:static sm:flex-row"
        v-if="mobileMenuActive"
      >
        <li class="cursor-pointer rounded bg-gray-900 px-2 py-1 text-gray-300">
          Dashboard
        </li>
        <li
          class="cursor-pointer rounded px-2 py-1 text-gray-300 hover:bg-gray-500 hover:text-gray-100"
        >
          Team
        </li>
        <li
          class="cursor-pointer rounded px-2 py-1 text-gray-300 hover:bg-gray-500 hover:text-gray-100"
        >
          Project
        </li>
        <li
          class="cursor-pointer rounded px-2 py-1 text-gray-300 hover:bg-gray-500 hover:text-gray-100"
        >
          Calendar
        </li>
      </ul>
    </div>
    <div class="flex items-center gap-2">
      <svg
        class="h-6 w-6"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        aria-hidden="true"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0"
        ></path>
      </svg>
      <div class="relative">
        <button @click="active = !active">
          <img
            class="h-10 w-10 rounded-full ring-2 ring-white ring-offset-2 ring-offset-gray-700"
            src="https://avatars.githubusercontent.com/u/2721809?v=4"
            alt="Alan"
          />
        </button>
        <ul
          class="absolute right-0 top-full flex min-w-[175px] flex-col bg-white text-gray-800"
          v-if="active"
        >
          <li class="p-2 hover:bg-gray-100">Your Profile</li>
          <li class="p-2 hover:bg-gray-100">Settings</li>
          <li class="p-2 hover:bg-gray-100">Signout</li>
        </ul>
      </div>
    </div>
  </header>
</template>
