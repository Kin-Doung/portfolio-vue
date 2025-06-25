<template>
  <header class="bg-white shadow sticky top-0 z-50">
    <nav class="container mx-auto px-4 py-4 flex justify-between items-center">
      <!-- Logo -->
      <h1 class="text-2xl font-bold text-indigo-600">Kin Doung</h1>

      <!-- Desktop Menu -->
      <ul class="hidden md:flex space-x-6 text-base font-medium text-gray-700">
        <li>
          <router-link to="/" class="hover:text-indigo-600 transition duration-300">Home</router-link>
        </li>
        <li>
          <router-link to="/about" class="hover:text-indigo-600 transition duration-300">About</router-link>
        </li>
        <li>
          <router-link to="/projects" class="hover:text-indigo-600 transition duration-300">Projects</router-link>
        </li>
        <li>
          <router-link to="/contact" class="hover:text-indigo-600 transition duration-300">Contact</router-link>
        </li>
      </ul>

      <!-- Mobile Menu Button -->
      <button @click="toggleMenu" class="md:hidden focus:outline-none">
        <svg class="w-6 h-6 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16M4 18h16"
          />
        </svg>
      </button>
    </nav>

    <!-- Mobile Menu -->
    <div v-if="isOpen" class="md:hidden px-4 pb-4">
      <ul class="space-y-2 text-base font-medium text-gray-700">
        <li>
          <router-link to="/" @click="closeMenu" class="block hover:text-indigo-600">Home</router-link>
        </li>
        <li>
          <router-link to="/about" @click="closeMenu" class="block hover:text-indigo-600">About</router-link>
        </li>
        <li>
          <router-link to="/projects" @click="closeMenu" class="block hover:text-indigo-600">Projects</router-link>
        </li>
        <li>
          <router-link to="/contact" @click="closeMenu" class="block hover:text-indigo-600">Contact</router-link>
        </li>
      </ul>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue'

const isOpen = ref(false)

const toggleMenu = () => {
  isOpen.value = !isOpen.value
}

const closeMenu = () => {
  isOpen.value = false
}
</script>
