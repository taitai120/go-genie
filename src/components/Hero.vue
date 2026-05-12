<script setup>
import heroImage from "../assets/ecosystem_horizontal 1.png";
</script>

<template>
  <section class="relative pt-16 overflow-hidden hero-gradient">
    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pt-12 sm:pt-16">
      <div class="text-center max-w-6xl mx-auto">
        <h1
          class="text-3xl sm:text-4xl lg:text-[40px] font-medium text-white leading-tight"
        >
          Measure and Reduce Your Logistics Carbon Footprint
        </h1>
        <p class="text-white/90 text-base sm:text-lg mb-8 max-w-2xl mx-auto">
          Track emissions, gain real-time insights, and make smarter, more
          sustainable logistics decisions.
        </p>
        <a
          href="#"
          class="hero-button inline-flex items-center gap-2 px-6 py-2 rounded-lg transition-all hover:opacity-90 bg-white text-brand font-medium text-[17px] leading-[26px] capitalize"
        >
          Explore Sustainability Solutions
          <svg
            class="w-5 h-5"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M9 5l7 7-7 7"
            />
          </svg>
        </a>
      </div>
    </div>

    <!-- Hero Image -->
    <div class="relative w-full">
      <img
        :src="heroImage"
        alt="GO-GENIE Ecosystem"
        class="w-full h-auto object-cover"
      />
      <!-- Gradient overlay at bottom to blend with next section -->
      <div
        class="absolute bottom-0 left-0 right-0 h-24 bg-gradient-to-t from-body-bg to-transparent"
      ></div>
    </div>
  </section>
</template>

<style scoped>
.hero-gradient {
  background: linear-gradient(
    0deg,
    var(--color-brand-dark) -46.75%,
    var(--color-brand) 63.31%
  );
}

.hero-button {
  box-shadow:
    5px 8px 12px 0px #0a63a124,
    -4px -4px 12px 0px #036ab133 inset,
    6px 6px 8px 0px #ffffff1a inset;
}
</style>
