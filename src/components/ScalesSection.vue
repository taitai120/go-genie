<script setup>
import dataDrivenImage from "../assets/data-driven.png";
import scalableSolutionsImage from "../assets/scalable-solutions.png";
import realImpactImage from "../assets/real-impact.png";

const features = [
  {
    title: "Data-Driven Insights",
    description: "Make informed decisions with accurate carbon tracking data.",
    image: dataDrivenImage,
  },
  {
    title: "Scalable Solutions",
    description:
      "Apply sustainability practices across your entire logistics network.",
    image: scalableSolutionsImage,
  },
  {
    title: "Real Impact",
    description: "Reduce emissions while maintaining operational efficiency.",
    image: realImpactImage,
  },
];
</script>

<template>
  <section class="py-16 sm:py-24 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-12">
        <h2 class="text-2xl sm:text-3xl lg:text-4xl text-heading font-medium">
          Sustainability That
          <span class="text-brand">Scales with Your Business</span>
        </h2>
        <p class="text-gray-600 mt-4 max-w-2xl mx-auto">
          Reduce emissions, improve efficiency, and operate more responsibly
          with GO-GENIE®.
        </p>
      </div>

      <!-- Feature Cards -->
      <div class="grid md:grid-cols-3 gap-8">
        <div
          v-for="feature in features"
          :key="feature.title"
          class="text-center"
        >
          <!-- Image -->
          <div class="w-32 h-32 mx-auto mb-6 flex items-center justify-center">
            <img
              :src="feature.image"
              :alt="feature.title"
              class="max-w-full max-h-full object-contain"
            />
          </div>

          <h3 class="text-lg font-semibold text-heading-solid mb-2">
            {{ feature.title }}
          </h3>
          <p class="text-gray-600 text-sm">{{ feature.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>
