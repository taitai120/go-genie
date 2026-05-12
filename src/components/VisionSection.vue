<script setup>
import sceneryImage from "../assets/scenery 1.png";
</script>

<template>
  <section class="py-16 sm:py-24 bg-body-bg">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-12">
        <p
          class="font-semibold text-sm uppercase tracking-wider mb-2 text-brand"
        >
          Our Vision
        </p>
        <h2 class="text-2xl sm:text-3xl lg:text-4xl text-heading font-medium">
          Built for Measure Sustainability
        </h2>
      </div>

      <!-- Scenery Image -->
      <div class="max-w-4xl mx-auto">
        <img
          :src="sceneryImage"
          alt="GO-GENIE Sustainability"
          class="w-full h-auto rounded-3xl shadow-lg"
        />
      </div>

      <!-- Description - overlaps image, wider than image -->
      <div class="max-w-5xl mx-auto relative">
        <div
          class="description-box bg-white rounded-2xl px-8 py-6 sm:px-12 sm:py-8"
        >
          <p class="text-center text-lg leading-relaxed font-normal text-heading">
            At GO-GENIE®, sustainability starts with understanding your impact.
            We provide accurate, transparent carbon data and actionable insights
            so businesses can measure emissions, benchmark performance, and make
            informed decisions. Turning data into measurable, real-world impact.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.description-box {
  box-shadow: 5px -8px 18px 0px #0a63a11f;
}
</style>
