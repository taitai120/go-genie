<script setup>
import iconBolt from "../assets/tabler-icon-bolt.png";
import iconEye from "../assets/tabler-icon-eye.png";
import iconBuilding from "../assets/tabler-icon-building-warehouse.png";

const features = [
  {
    icon: iconBolt,
    iconBg: "bg-icon-blue",
    title: "Optimise Delivery Routes",
    description:
      "Reduce emissions by optimising routes and improving delivery efficiency.",
  },
  {
    icon: iconEye,
    iconBg: "bg-icon-teal",
    title: "Monitor Environmental Impact",
    description:
      "Track carbon emissions across shipments with real-time insights.",
  },
  {
    icon: iconBuilding,
    iconBg: "bg-icon-yellow",
    title: "Achieve Sustainability Goals",
    description:
      "Set targets and measure progress toward your sustainability objectives.",
  },
];
</script>

<template>
  <section class="py-16 sm:py-24 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-12">
        <h2 class="text-2xl sm:text-3xl lg:text-4xl text-heading font-medium mb-2">
          Real-Time Carbon Tracking
        </h2>
        <p class="text-2xl sm:text-3xl lg:text-4xl text-brand">
          for Every Delivery
        </p>
        <p class="text-gray-600 mt-4 max-w-2xl mx-auto">
          Monitor emissions, optimise routes, and improve sustainability across
          your logistics operations.
        </p>
      </div>

      <!-- Feature Cards -->
      <div class="grid md:grid-cols-3 gap-6 sm:gap-8 mb-12">
        <div
          v-for="feature in features"
          :key="feature.title"
          class="feature-card text-left p-6 sm:p-8 rounded-2xl bg-white"
        >
          <!-- Icon -->
          <div
            class="w-14 h-14 mb-6 rounded-xl flex items-center justify-center"
            :class="feature.iconBg"
          >
            <img :src="feature.icon" :alt="feature.title" class="w-7 h-7" />
          </div>
          <h3 class="text-lg font-semibold text-heading-solid mb-3">
            {{ feature.title }}
          </h3>
          <p class="text-gray-500 text-sm leading-relaxed">
            {{ feature.description }}
          </p>
        </div>
      </div>

      <!-- CTA Button -->
      <div class="text-center">
        <a
          href="#"
          class="cta-button inline-flex items-center gap-2 border border-brand text-brand px-6 py-2 rounded-lg font-medium transition-colors hover:bg-brand hover:text-white"
        >
          Book A Demo
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
              d="M17 8l4 4m0 0l-4 4m4-4H3"
            />
          </svg>
        </a>
      </div>
    </div>
  </section>
</template>

<style scoped>
.feature-card {
  box-shadow:
    5px 8px 9px 0px #0a63a114,
    -8px -8px 16px 0px #036ab112 inset;
}

.cta-button {
  box-shadow: 5px 8px 9px 0px #0a63a114;
}
</style>
