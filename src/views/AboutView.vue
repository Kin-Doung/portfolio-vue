<template>
  <section class="p-8 bg-gray-100 min-h-screen">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-4xl font-bold text-indigo-600 mb-10 text-center">
        About Me
      </h2>

      <div
        class="bg-white rounded-lg shadow-lg p-6 mb-8 max-w-prose mx-auto text-gray-700"
      >
        <p>
          My name is <strong>Kin Doung</strong>, and I am a student at Passerelles Numériques Cambodia (PNC). During my
          studies, I have worked on several projects like a POS system, a Note Taker app,
          face detection, and hosting projects on AWS.
        </p>
      </div>

      <!-- Grid container for 2-column layout -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 max-w-6xl mx-auto">
        <!-- Education Card -->
        <div
          class="bg-white rounded-lg shadow-md p-6 border border-indigo-200"
        >
          <h3
            class="text-2xl font-semibold mb-4 flex items-center text-indigo-600 border-b-2 border-indigo-300 pb-2"
          >
            <i class="fas fa-graduation-cap mr-3"></i> Education
          </h3>
          <ul class="list-disc pl-6 space-y-2 text-gray-700">
            <li>Associate Degree, PNC (2024 - 2025)</li>
            <li>BAC II, Chub Vary High School (2020 - 2023)</li>
          </ul>
        </div>

        <!-- Workshops Card -->
        <div
          class="bg-white rounded-lg shadow-md p-6 border border-indigo-200"
        >
          <h3
            class="text-2xl font-semibold mb-4 flex items-center text-indigo-600 border-b-2 border-indigo-300 pb-2"
          >
            <i class="fas fa-laptop-code mr-3"></i> Workshops
          </h3>
          <ul class="list-disc pl-6 space-y-1 text-gray-700">
            <li>Product Owner Workshop (Jan 2025)</li>
            <li>UX/UI Design Workshop (Feb & Mar 2025)</li>
            <li>Data Analytics Workshop (Mar 2025)</li>
            <li>Project Management Workshop (Feb 2025)</li>
          </ul>
        </div>

        <!-- Hard Skills Card -->
        <div
          class="bg-white rounded-lg shadow-md p-6 border border-indigo-200"
        >
          <h3
            class="text-2xl font-semibold mb-4 flex items-center text-indigo-600 border-b-2 border-indigo-300 pb-2"
          >
            <i class="fas fa-tools mr-3"></i> Hard Skills
          </h3>
          <p class="text-gray-700">
            HTML, CSS, Bootstrap 5, Tailwind CSS, JavaScript, PHP, MySQL, Firebase, Node.js,
            OOP with TypeScript, Vue.js, Laravel, Python, Power BI
          </p>
        </div>

        <!-- Soft Skills Card -->
        <div
          class="bg-white rounded-lg shadow-md p-6 border border-indigo-200"
        >
          <h3
            class="text-2xl font-semibold mb-4 flex items-center text-indigo-600 border-b-2 border-indigo-300 pb-2"
          >
            <i class="fas fa-user-friends mr-3"></i> Soft Skills
          </h3>
          <p class="text-gray-700">
            Teamwork, Communication, Time Management, Research, Problem Solving, Project Management
          </p>
        </div>

        <!-- Tools Card -->
        <div
          class="bg-white rounded-lg shadow-md p-6 border border-indigo-200"
        >
          <h3
            class="text-2xl font-semibold mb-4 flex items-center text-indigo-600 border-b-2 border-indigo-300 pb-2"
          >
            <i class="fas fa-cogs mr-3"></i> Tools
          </h3>
          <p class="text-gray-700">
            Git, GitHub, Jira, Figma, Netlify, Vercel, AWS, Ubuntu, Postman, MS Office
          </p>
        </div>

        <!-- Languages Card -->
        <div
          class="bg-white rounded-lg shadow-md p-6 border border-indigo-200"
        >
          <h3
            class="text-2xl font-semibold mb-4 flex items-center text-indigo-600 border-b-2 border-indigo-300 pb-2"
          >
            <i class="fas fa-language mr-3"></i> Languages
          </h3>
          <p class="text-gray-700">
            English (Pre-Intermediate), Khmer (Mother Tongue)
          </p>
        </div>
      </div>
    </div>
  </section>
</template>
  