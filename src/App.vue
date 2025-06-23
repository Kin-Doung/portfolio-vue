<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header class="bg-white shadow-md sticky top-0 z-50">
    <div class="container mx-auto flex justify-between items-center px-4 py-3">
      <!-- Logo -->
      <h1 class="text-xl font-bold text-indigo-600">My Portfolio</h1>

      <!-- Navigation -->
      <nav class="flex space-x-4">
        <RouterLink
          to="/"
          class="text-gray-600 hover:text-indigo-600 font-medium"
          active-class="text-indigo-600 font-bold"
        >Home</RouterLink>

        <RouterLink
          to="/about"
          class="text-gray-600 hover:text-indigo-600 font-medium"
          active-class="text-indigo-600 font-bold"
        >About</RouterLink>

        <RouterLink
          to="/service"
          class="text-gray-600 hover:text-indigo-600 font-medium"
          active-class="text-indigo-600 font-bold"
        >Service</RouterLink>

        <RouterLink
          to="/contact"
          class="text-gray-600 hover:text-indigo-600 font-medium"
          active-class="text-indigo-600 font-bold"
        >Contact</RouterLink>
      </nav>
    </div>
  </header>

  <!-- Content -->
  <main class="p-4">
    <RouterView />
  </main>
</template>
