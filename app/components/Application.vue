<script setup lang="ts"></script>

<template>
  <div class="flex flex-col md:flex-row items-center justify-between container">
    <div
      class="flex flex-col items-center md:items-start text-center md:text-left space-y-4"
    >
      <p class="text-3xl font-bold">Foodly is Available for Android and IOS</p>
      <div class="flex flex-col md:flex-row">
        <NuxtImg
          class="hover:rotate-6 transition-transform duration-300 rounded-md"
          width="200px"
          src="/images/play_store.png"
          format="webp"
          alt="Play Store"
        />
        <NuxtImg
          class="hover:rotate-6 transition-transform duration-300 rounded-md"
          width="200px"
          src="/images/app_store.png"
          format="webp"
          alt="App Store"
        />
      </div>
    </div>

    <div class="mt-6 md:mt-0">
      <NuxtImg
        class="w-64 h-auto rounded-3xl"
        src="/images/mobile_bike.gif"
        alt="Mobile Bike GIF"
      />
    </div>
  </div>
</template>

<style scoped></style>
