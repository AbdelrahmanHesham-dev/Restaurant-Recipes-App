<script setup lang="ts">
import { ref } from "vue";

const isMenuOpen = ref(false);
</script>

<template>
  <header class="py-4 border-b">
    <nav class="flex container items-center">
      <NuxtLink to="/" class="flex gap-1 items-center">
        <NuxtImg width="45px" src="/images/logo.png" format="webp" alt="" />
        <span class="text-3xl font-[900]">Foodie</span>
      </NuxtLink>

      <button
        class="ml-auto md:hidden text-3xl"
        @click="isMenuOpen = !isMenuOpen"
        aria-label="Toggle Menu"
      >
        ☰
      </button>

      <ul
        :class="[
          'flex gap-6 text-xl font-bold capitalize',
          isMenuOpen
            ? 'flex flex-col absolute top-16 right-0 bg-white w-full p-4 shadow-lg'
            : 'hidden',
          'md:flex md:static md:flex-row md:ml-auto md:shadow-none md:bg-transparent',
        ]"
      >
        <li>
          <NuxtLink to="/" class="block py-2 md:py-0">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/recipes" class="block py-2 md:py-0">Recipes</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about" class="block py-2 md:py-0">About</NuxtLink>
        </li>
      </ul>
    </nav>
  </header>
</template>
