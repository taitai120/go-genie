<script setup>
import ecosystemImage from "../assets/ecosystem_sep2025_8000x4500 1.png";
</script>

<template>
  <section class="py-16 sm:py-24 bg-body-bg">
    <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Image on top -->
      <div class="flex justify-center">
        <img
          :src="ecosystemImage"
          alt="GO-GENIE Ecosystem"
          class="w-full max-w-4xl h-auto object-contain"
        />
      </div>

      <!-- Card overlapping image -->
      <div class="relative -mt-16 sm:-mt-24 z-10 max-w-4xl mx-auto">
        <div class="cta-card bg-white rounded-2xl p-8 sm:p-12 text-center">
          <h2 class="text-2xl sm:text-3xl lg:text-4xl text-heading font-medium mb-2">
            Start Building a More Sustainable
          </h2>
          <p class="text-2xl sm:text-3xl lg:text-4xl text-brand mb-6">
            Logistics Operation
          </p>
          <p class="text-gray-500 mb-8 max-w-xl mx-auto">
            Take control of your emissions, meet sustainability goals, and
            create measurable impact. GO SMART, GO GREEN, GO-GENIE®
          </p>
          <a
            href="#"
            class="cta-button inline-flex items-center gap-2 bg-brand text-white px-6 py-3 rounded-lg font-medium transition-colors hover:opacity-90"
          >
            Talk To Our Team
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.cta-card {
  box-shadow:
    2px 2px 19px 0px #385e7829,
    -8px -8px 30px 0px #0f507e14 inset,
    8px 8px 30px 0px #ffffff66 inset;
}

.cta-button {
  box-shadow:
    5px 5px 14px 0px #013f722e,
    -6px -6px 14px 0px #00223f42 inset,
    6px 6px 14px 0px #80b1d3 inset;
}
</style>
