<script setup>
import trackProgressImage from "../assets/Image Container.png";
import reportsImage from "../assets/Reports Image.png";
import showcaseImage from "../assets/Showcase Image.png";

const features = [
  {
    title: "Track Progress",
    description:
      "Monitor your progress towards sustainability and certification targets.",
    image: trackProgressImage,
  },
  {
    title: "Generate Reports",
    description:
      "Create detailed reports for audits, compliance, and internal tracking.",
    image: reportsImage,
  },
  {
    title: "Showcase Achievements",
    description:
      "Highlight your sustainability efforts and build trust with customers.",
    image: showcaseImage,
  },
];
</script>

<template>
  <section class="py-16 sm:py-24 bg-body-bg">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-20">
        <h2 class="text-2xl sm:text-3xl lg:text-4xl text-heading font-medium mb-2">
          Simplify Sustainability
        </h2>
        <p class="text-2xl sm:text-3xl lg:text-4xl text-brand">
          Reporting and Compliance
        </p>
        <p class="text-gray-600 mt-4 max-w-2xl mx-auto">
          Track progress, generate reports and meet sustainability standards
          with ease.
        </p>
      </div>

      <!-- Feature Cards with Images -->
      <div class="space-y-16 sm:space-y-20">
        <div
          v-for="feature in features"
          :key="feature.title"
          class="relative"
        >
          <!-- Card (below image) -->
          <div class="feature-card bg-white rounded-2xl relative z-10">
            <div class="flex flex-col md:flex-row items-center min-h-[160px]">
              <!-- Content -->
              <div class="flex-1 p-8 sm:p-12 md:pr-[280px]">
                <h3 class="text-xl sm:text-2xl font-semibold text-heading-solid mb-3">
                  {{ feature.title }}
                </h3>
                <p class="text-gray-500 leading-relaxed">
                  {{ feature.description }}
                </p>
              </div>
            </div>
          </div>

          <!-- Image (on top of card, extends outside) -->
          <div class="hidden md:block absolute right-8 top-1/2 -translate-y-1/2 z-20">
            <img
              :src="feature.image"
              :alt="feature.title"
              class="h-[260px] object-contain"
            />
          </div>

          <!-- Mobile image -->
          <div class="md:hidden flex justify-center -mt-4">
            <img
              :src="feature.image"
              :alt="feature.title"
              class="h-48 object-contain"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.feature-card {
  box-shadow:
    5px 5px 14px 0px #0A63A114,
    2px 2px 19px 0px #385E7829,
    -8px -8px 30px 0px #0F507E14 inset,
    8px 8px 30px 0px #FFFFFF66 inset;
}
</style>
