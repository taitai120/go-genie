<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import VisionSection from './components/VisionSection.vue'
import CarbonTracking from './components/CarbonTracking.vue'
import ReportingSection from './components/ReportingSection.vue'
import ScalesSection from './components/ScalesSection.vue'
import CtaSection from './components/CtaSection.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="min-h-screen bg-white">
    <Header />
    <main>
      <Hero />
      <VisionSection />
      <CarbonTracking />
      <ReportingSection />
      <ScalesSection />
      <CtaSection />
    </main>
    <Footer />
  </div>
</template>
