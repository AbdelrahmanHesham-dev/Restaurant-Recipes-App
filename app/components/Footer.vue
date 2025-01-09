<script setup lang="ts"></script>

<template>
  <footer class="bg-[#f1f1f1] text-gray-800 py-10">
    <div class="container mx-auto grid grid-cols-1 md:grid-cols-3 gap-10">
      <div>
        <NuxtLink to="/" class="flex gap-1 items-center mb-5">
          <NuxtImg width="45px" src="/images/logo.png" format="webp" alt="" />
          <span class="text-3xl font-[900]">Foodie</span>
        </NuxtLink>
        <p class="text-gray-600">
          Foodie brings you the finest dishes from around the world. Enjoy a
          unique dining experience with unforgettable flavors.
        </p>
      </div>

      <div>
        <h3 class="text-xl font-bold mb-4 text-black">Quick Links</h3>
        <ul class="space-y-2">
          <li>
            <NuxtLink to="#hero" class="hover:text-dodgeroll-gold"
              >Home</NuxtLink
            >
          </li>
          <li>
            <NuxtLink to="#recipes" class="hover:text-dodgeroll-gold"
              >Menu</NuxtLink
            >
          </li>
          <li>
            <NuxtLink to="#about" class="hover:text-dodgeroll-gold"
              >About Us</NuxtLink
            >
          </li>
        </ul>
      </div>

      <div>
        <h3 class="text-xl font-bold mb-4 text-black">Follow Us</h3>
        <div class="flex space-x-4 mb-6">
          <NuxtLink
            to="#"
            aria-label="Facebook"
            class="hover:text-dodgeroll-gold"
          >
            <Icon
              name="i-mdi-facebook"
              class="text-gray-600 hover:text-dodgeroll-gold text-2xl"
            />
          </NuxtLink>
          <NuxtLink
            to="#"
            aria-label="Twitter"
            class="hover:text-dodgeroll-gold"
          >
            <Icon
              name="i-mdi-twitter"
              class="text-gray-600 hover:text-dodgeroll-gold text-2xl"
            />
          </NuxtLink>
          <NuxtLink
            to="#"
            aria-label="Instagram"
            class="hover:text-dodgeroll-gold"
          >
            <Icon
              name="i-mdi-instagram"
              class="text-gray-600 hover:text-dodgeroll-gold text-2xl"
            />
          </NuxtLink>
        </div>
        <h3 class="text-xl font-bold mb-4 text-black">
          Subscribe to Our Newsletter
        </h3>
        <form class="flex">
          <input
            type="email"
            placeholder="Enter your email"
            class="px-1 py-2 rounded-l bg-gray-200 text-gray-800 focus:outline-none"
          />
          <button
            type="submit"
            class="px-4 py-2 rounded-r bg-dodgeroll-gold hover:bg-yellow-500 text-white font-bold"
          >
            Subscribe
          </button>
        </form>
      </div>
    </div>

    <div class="text-center text-gray-600 mt-10">
      <p>
        © 2025 <span class="text-dodgeroll-gold">Foodie</span>. All Rights
        Reserved.
      </p>
    </div>
  </footer>
</template>
