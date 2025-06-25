<template>
  <section class="p-8 bg-gray-50 min-h-screen">
    <div class="max-w-5xl mx-auto">
      <h2 class="text-3xl font-bold text-indigo-600 mb-10 border-b-4 border-indigo-600 pb-2">
        Projects
      </h2>

      <div
        v-for="(project, index) in projects"
        :key="index"
        class="bg-white rounded-xl shadow-md p-6 mb-8 hover:shadow-xl transition-shadow duration-300"
      >
        <!-- Title with folder icon -->
        <h3 class="text-xl font-semibold mb-2 flex items-center text-gray-900">
          <FolderIcon class="w-5 h-5 text-indigo-600 mr-2" />
          {{ project.title }}
        </h3>

        <!-- Date with calendar icon -->
        <p class="text-sm text-gray-500 mb-3 flex items-center">
          <CalendarIcon class="w-4 h-4 mr-1" />
          {{ project.date }}
        </p>

        <p class="text-gray-700 mb-3">{{ project.description }}</p>

        <!-- Tech stack with code icon -->
        <p v-if="project.tech" class="mb-3 text-gray-700 flex items-center">
          <CodeIcon class="w-4 h-4 mr-1" />
          <strong class="mr-1">Tech:</strong> {{ project.tech }}
        </p>

        <!-- Link with external link icon -->
        <a
          v-if="project.link"
          :href="project.link"
          target="_blank"
          rel="noopener"
          class="text-indigo-600 underline hover:text-indigo-800 font-medium inline-flex items-center"
        >
          View Code
          <ExternalLinkIcon class="w-4 h-4 ml-1" />
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
const projects = [
  {
    title: 'POS-System - Virtual Company Project',
    date: 'Feb 25 – May 2, 2025',
    description: 'Developed a POS system to help customers manage sales and inventory.',
    tech: 'HTML, CSS, JavaScript, Bootstrap 5, PHP, MySQL',
    link: 'https://github.com/Kin-Doung/POS-SYSTEM-G5',
  },
  {
    title: 'Note-Taker App',
    date: 'Jan 12 – Jan 26, 2025',
    description: 'Created a note-taking app for writing and organizing tasks.',
    tech: 'JavaScript, HTML, CSS, Firebase',
    link: 'https://github.com/Kin-Doung/Note-taker-app---G10',
  },
  {
    title: 'Face Detection - Algorithm Project',
    date: 'Nov 11 – Nov 20, 2024',
    description: 'Implemented check-in and check-out tracking using Python algorithms.',
    link: 'https://github.com/poleaktheng065/Face_Scan_Team_6',
  },
  {
    title: 'Clinic Service - Web Design',
    date: 'Oct 17 – Nov 5, 2024',
    description: 'Designed a website for clinic services using HTML, CSS, and SASS.',
    link: 'https://github.com/darinhoy/clinic-service-A6',
  },
  {
    title: 'Hosting WordPress - Software Deployment',
    date: 'Dec 31 – Jan 5, 2025',
    description: 'Deployed WordPress site using MobaXterm and AWS.',
  },
]

// Icon components using inline SVGs:
const FolderIcon = {
  props: ['class'],
  template: `
    <svg :class="class" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
      viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <path d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-7l-2-2H5a2 2 0 00-2 2z"/>
    </svg>
  `
}

const CalendarIcon = {
  props: ['class'],
  template: `
    <svg :class="class" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
      viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <rect width="18" height="18" x="3" y="4" rx="2" ry="2"/>
      <line x1="16" y1="2" x2="16" y2="6"/>
      <line x1="8" y1="2" x2="8" y2="6"/>
      <line x1="3" y1="10" x2="21" y2="10"/>
    </svg>
  `
}

const CodeIcon = {
  props: ['class'],
  template: `
    <svg :class="class" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
      viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <polyline points="16 18 22 12 16 6"/>
      <polyline points="8 6 2 12 8 18"/>
    </svg>
  `
}

const ExternalLinkIcon = {
  props: ['class'],
  template: `
    <svg :class="class" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
      viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <path d="M18 13v6a2 2 0 01-2 2H6a2 2 0 01-2-2V8a2 2 0 012-2h6"/>
      <polyline points="15 3 21 3 21 9"/>
      <line x1="10" y1="14" x2="21" y2="3"/>
    </svg>
  `
}
</script>
