<script setup>
import { ref } from 'vue'
import logoWhite from '../assets/White.png'

const isMenuOpen = ref(false)

const navItems = [
  { name: 'Services', hasDropdown: true },
  { name: 'Solutions', hasDropdown: true },
  { name: 'About', hasDropdown: true },
  { name: 'Help & Guides', hasDropdown: true },
]
</script>

<template>
  <header class="fixed top-0 left-0 right-0 z-50 bg-brand">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <!-- Logo + Navigation (40px gap) -->
        <div class="flex items-center gap-10">
          <a href="/" class="flex items-center">
            <img :src="logoWhite" alt="GO-GENIE" class="h-8 w-auto" />
          </a>

          <!-- Desktop Navigation -->
          <nav class="hidden md:flex items-center gap-8">
          <a
            v-for="item in navItems"
            :key="item.name"
            href="#"
            class="text-white text-sm font-medium flex items-center gap-1 transition-colors hover:text-white/80"
          >
            {{ item.name }}
            <svg v-if="item.hasDropdown" class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"/>
            </svg>
          </a>
        </nav>
        </div>

        <!-- Right Side -->
        <div class="flex items-center gap-3">
          <!-- Track Your Parcel Button -->
          <a
            href="#"
            class="hidden sm:flex items-center gap-2 px-4 py-2 rounded-lg text-sm font-semibold transition-colors text-white border border-white hover:bg-white hover:text-brand"
          >
            Track Your Parcel
          </a>

          <!-- Sign In Button -->
          <a
            href="#"
            class="hidden sm:flex items-center gap-2 bg-white text-brand px-4 py-2 rounded-lg text-sm font-semibold transition-colors hover:bg-gray-100"
          >
            Sign In
          </a>

          <!-- Language Selector -->
          <button class="text-white p-2 hover:bg-white/10 rounded-lg transition-colors flex items-center gap-1">
            <img src="https://flagcdn.com/w20/gb.png" alt="EN" class="w-5 h-4 rounded-sm">
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"/>
            </svg>
          </button>

          <!-- Mobile menu button -->
          <button @click="isMenuOpen = !isMenuOpen" class="md:hidden text-white p-2">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path v-if="!isMenuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
              <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"/>
            </svg>
          </button>
        </div>
      </div>

      <!-- Mobile Navigation -->
      <div v-if="isMenuOpen" class="md:hidden pb-4">
        <a
          v-for="item in navItems"
          :key="item.name"
          href="#"
          class="block py-2 text-white text-sm font-medium"
        >
          {{ item.name }}
        </a>
        <div class="mt-3 space-y-2">
          <a href="#" class="block border border-white text-white px-4 py-2 rounded-lg text-sm font-semibold text-center">
            Track Your Parcel
          </a>
          <a href="#" class="block bg-white text-brand px-4 py-2 rounded-lg text-sm font-semibold text-center">
            Sign In
          </a>
        </div>
      </div>
    </div>
  </header>
</template>
