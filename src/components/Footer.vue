<template>
  <footer class="bg-gray-800 text-white py-6 mt-12">
    <div class="container mx-auto text-center">
      <p class="text-sm">
        &copy; {{ currentYear }} Kin Doung. All rights reserved.
      </p>
      <div class="flex justify-center space-x-4 mt-2">
        <a href="https://github.com/yourusername" target="_blank" class="hover:text-indigo-400">
          GitHub
        </a>
        <a href="https://linkedin.com/in/yourprofile" target="_blank" class="hover:text-indigo-400">
          LinkedIn
        </a>
        <a href="mailto:youremail@example.com" class="hover:text-indigo-400">
          Email
        </a>
      </div>
    </div>
  </footer>
</template>

<script setup>
const currentYear = new Date().getFullYear()
</script>
