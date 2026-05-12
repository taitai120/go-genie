<script setup>
import logoWhite from "../assets/White.png";
import footer1 from "../assets/footer-1.png";
import footer2 from "../assets/footer-2.png";
import footer3 from "../assets/footer-3.png";
import footer4 from "../assets/footer-4.png";

const footerLinks = {
  services: {
    title: "Services",
    links: ["Last-Mile Delivery", "Warehousing", "Fulfilment"],
  },
  solutions: {
    title: "Solutions",
    links: ["Merchants", "Service Providers", "Gig Workers"],
  },
  about: {
    title: "About",
    links: ["GO-GENIE®", "Our Ecosystem", "Sustainability", "Newsroom"],
  },
  help: {
    title: "Help & Guides",
    links: ["Help Center", "Contact Us"],
  },
  quickLinks: {
    title: "Quick Links",
    links: ["Privacy Policy", "Terms of Service", "Data Retention Policy"],
  },
};

const awards = [
  "Brands For Good 2025 - Honouree",
  "SPBA 2025 - Promising Brands",
  "SPBA 2025 - Transformation Efforts",
];

const chambers = [
  "Member of Singapore Chinese Chamber of Commerce & Industry (SCCCI)",
  "Member of Singapore Business Federation (SBF)",
];

const partnerLogos = [footer1, footer2, footer3, footer4];
</script>

<template>
  <footer>
    <!-- Main Footer - Blue Section -->
    <div class="bg-brand">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
        <!-- Logo -->
        <div class="mb-8">
          <img :src="logoWhite" alt="GO-GENIE" class="h-8 w-auto" />
        </div>

        <!-- Divider -->
        <div class="border-t border-white/20 mb-8"></div>

        <!-- Links Grid -->
        <div class="grid grid-cols-2 md:grid-cols-5 gap-8 mb-12">
          <div v-for="(section, key) in footerLinks" :key="key">
            <h4 class="font-semibold text-white mb-4 text-sm">
              {{ section.title }}
            </h4>
            <ul class="space-y-3">
              <li v-for="link in section.links" :key="link">
                <a
                  href="#"
                  class="text-white/70 hover:text-white text-sm transition-colors"
                >
                  {{ link }}
                </a>
              </li>
            </ul>
          </div>
        </div>

        <!-- Divider -->
        <div class="border-t border-white/20 mb-8"></div>

        <!-- Address & Social -->
        <div
          class="flex flex-col md:flex-row justify-between items-start md:items-center gap-6"
        >
          <p class="text-white/80 text-sm max-w-[250px]">
            <span class="font-medium">Singapore Address:</span> 1234 Building,
            Random Rd, Singapore, 17890123
          </p>
          <p class="text-white/80 text-sm max-w-[280px]">
            <span class="font-medium">Vietnam Address:</span> 1234 Rd, Random
            District, Ho Chi Minh City, Vietnam
          </p>
          <div class="text-right">
            <p class="text-white/80 text-sm mb-3">Follow us and keep updated</p>
            <div class="flex gap-3 justify-start">
              <!-- Facebook -->
              <a
                href="#"
                class="text-white hover:text-white/80 transition-colors"
              >
                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"
                  />
                </svg>
              </a>
              <!-- Instagram -->
              <a
                href="#"
                class="text-white hover:text-white/80 transition-colors"
              >
                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"
                  />
                </svg>
              </a>
              <!-- TikTok -->
              <a
                href="#"
                class="text-white hover:text-white/80 transition-colors"
              >
                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M12.525.02c1.31-.02 2.61-.01 3.91-.02.08 1.53.63 3.09 1.75 4.17 1.12 1.11 2.7 1.62 4.24 1.79v4.03c-1.44-.05-2.89-.35-4.2-.97-.57-.26-1.1-.59-1.62-.93-.01 2.92.01 5.84-.02 8.75-.08 1.4-.54 2.79-1.35 3.94-1.31 1.92-3.58 3.17-5.91 3.21-1.43.08-2.86-.31-4.08-1.03-2.02-1.19-3.44-3.37-3.65-5.71-.02-.5-.03-1-.01-1.49.18-1.9 1.12-3.72 2.58-4.96 1.66-1.44 3.98-2.13 6.15-1.72.02 1.48-.04 2.96-.04 4.44-.99-.32-2.15-.23-3.02.37-.63.41-1.11 1.04-1.36 1.75-.21.51-.15 1.07-.14 1.61.24 1.64 1.82 3.02 3.5 2.87 1.12-.01 2.19-.66 2.77-1.61.19-.33.4-.67.41-1.06.1-1.79.06-3.57.07-5.36.01-4.03-.01-8.05.02-12.07z"
                  />
                </svg>
              </a>
              <!-- X (Twitter) -->
              <a
                href="#"
                class="text-white hover:text-white/80 transition-colors"
              >
                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"
                  />
                </svg>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Awards Section - White Background -->
    <div class="bg-white py-12">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex flex-col lg:flex-row gap-12">
          <!-- Left side - Text -->
          <div class="lg:w-1/3">
            <h4 class="font-semibold text-[#262B43] mb-4 text-lg">
              Awards and Recognition
            </h4>
            <ul class="text-gray-600 text-sm space-y-2 mb-8">
              <li v-for="award in awards" :key="award">{{ award }}</li>
            </ul>

            <h4 class="font-semibold text-[#262B43] mb-4 text-lg">
              Business Chambers
            </h4>
            <ul class="text-gray-600 text-sm space-y-2">
              <li v-for="chamber in chambers" :key="chamber">{{ chamber }}</li>
            </ul>
          </div>

          <!-- Right side - Logos -->
          <div
            class="lg:w-2/3 flex flex-wrap items-center justify-center lg:justify-end gap-8"
          >
            <img
              v-for="(logo, index) in partnerLogos"
              :key="index"
              :src="logo"
              :alt="'Partner ' + (index + 1)"
              class="h-16 sm:h-20 w-auto object-contain"
            />
          </div>
        </div>
      </div>
    </div>

    <!-- Copyright - Brand Blue -->
    <div class="bg-brand py-4">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <p class="text-center text-white/80 text-sm">
          © 2026 GO-GENIE® All Rights Reserved.
        </p>
      </div>
    </div>
  </footer>
</template>
