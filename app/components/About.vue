<script setup lang="ts"></script>

<template>
  <section class="about-section py-16 px-4 bg-[#f1f1f1]">
    <div class="container mx-auto text-center">
      <h2 class="text-5xl font-bold text-dodgeroll-gold mb-6">
        About Our Restaurant
      </h2>
      <p class="text-lg text-gray-700 mb-8">
        Welcome to our restaurant! We believe in serving delicious, high-quality
        dishes made from the freshest ingredients. Our team is passionate about
        sharing our love for food, offering a unique dining experience with
        every bite.
      </p>
      <div class="flex flex-wrap justify-center gap-8">
        <div class="about-card p-6 bg-white rounded-lg shadow-lg">
          <div class="mb-6">
            <NuxtImg
              class="rotate-img"
              width="350px"
              src="/images/biryani2.png"
              format="webp"
              alt="Restaurant Vision"
            />
          </div>
          <h3 class="text-xl font-semibold text-dire-wolf">Our Vision</h3>
          <p class="text-gray-600 mt-4">
            To provide exceptional food experiences and bring people together
            through the love of great recipes. we have been creating
            unforgettable dining moments.
          </p>
        </div>
        <div class="about-card p-6 bg-white rounded-lg shadow-lg">
          <div class="mb-6">
            <NuxtImg
              class="rotate-img"
              width="200px"
              src="/images/biryani3.png"
              format="webp"
              alt="Restaurant Mission"
            />
          </div>
          <h3 class="text-xl font-semibold text-dire-wolf">Our Mission</h3>
          <p class="text-gray-600 mt-4">
            To craft mouthwatering recipes that not only taste great but also
            nourish your soul. Our aim is to inspire food lovers everywhere with
            creative and delightful dishes.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.about-section {
  background-color: #f7f7f7;
}

.about-card {
  max-width: 300px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.about-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

.rotate-img {
  animation: rotate 10s infinite linear;
}

@keyframes rotate {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

@media (max-width: 768px) {
  .about-card {
    max-width: 90%;
  }

  .rotate-img {
    width: 100%;
  }
}

@media (max-width: 480px) {
  .about-section {
    padding-top: 8px;
    padding-bottom: 8px;
  }

  .text-3xl {
    font-size: 2xl;
  }

  .text-lg {
    font-size: md;
  }
}
</style>
