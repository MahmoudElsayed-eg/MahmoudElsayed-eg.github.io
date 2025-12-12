<script setup></script>

<template>
  <main :dir="$i18n.locale == 'ar' ? 'rtl' : 'ltr'"
    class="p-4 flex flex-col gap-3 items-center justify-center max-w-5xl mx-auto">
    <h1 id="hello" class="mt-6 text-3xl font-semibold">{{ $t('hello') }}</h1>
    <h2 class="text-3xl font-semibold text-gray-400">{{ $t('job_title') }}</h2>
    <p class="text-gray-400">{{ $t('summary') }}</p>
    <a class="p-3 bg-green-900 rounded-lg" href="/Mahmoud_Elsayed.pdf" target="_blank">{{
      $t('cv')
    }}</a>
    <section class="">
      <RouterLink to="/projects" class="text-2xl font-bold text-gray-400 mb-6">{{ $t('projects') }}</RouterLink>
      <p class="mb-6 text-gray-500">{{ $t('projects_desc') }}</p>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="flex flex-col">
          <h3 class="text-lg font-semibold text-gray-500 mb-2">Web</h3>
          <ul class="list-disc ps-5 text-gray-600 space-y-2">
            <li>
              <a href="https://www.walltips.com/" target="_blank" class="hover:underline text-xl text-gray-300">
                {{ $t('walltips.title') }}
              </a>
              <p class="text-gray-500 mt-1">{{ $t('walltips.description') }}</p>
            </li>
            <li>
              <a href="https://www.foxprox.com/" target="_blank" class="hover:underline text-xl text-gray-300">
                {{ $t('foxprox.title') }}
              </a>
              <p class="text-gray-500 mt-1">{{ $t('foxprox.description') }}</p>
            </li>
            <li>
              <a href="https://masterfox.ae/" target="_blank" class="hover:underline text-xl text-gray-300">
                {{ $t('masterfox.title') }}
              </a>
              <p class="text-gray-500 mt-1">{{ $t('masterfox.description') }}</p>
            </li>
          </ul>
        </div>
        <div class="flex flex-col">
          <h3 class="text-lg font-semibold text-gray-500 mb-2">Android</h3>
          <ul class="list-disc ps-5 text-gray-600">
            <li>
              <a href="https://play.google.com/store/apps/details?id=com.mahmoudelsayed.prompt2pic&pli=1"
                target="_blank" class="hover:underline text-xl text-gray-300">
                {{ $t('prompt2pic.title') }}
              </a>
              <p class="text-gray-500 mt-1">{{ $t('prompt2pic.description') }}</p>
            </li>
          </ul>
        </div>
      </div>
    </section>
    <section class="mt-5 w-full mb-4">
      <h2 class="text-2xl font-bold text-gray-400 mb-4">{{ $t('skills') }}</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div>
          <h3 class="text-lg font-semibold text-gray-500 mb-2">Programming Languages</h3>
          <ul class="list-disc ps-5 text-gray-600">
            <li>PHP (Laravel, Symfony , Wordpress)</li>
            <li>Node.js (Express)</li>
            <li>TypeScript (Vue 3, React , Angular)</li>
            <li>Java/Kotlin (Android)</li>
            <li>SQL (MySQL, PostgreSQL , SQlite , SQl server)</li>
            <li>NoSQL (MongoDB)</li>
          </ul>
        </div>
        <div>
          <h3 class="text-lg font-semibold text-gray-500 mb-2">DevOps & Tooling</h3>
          <ul class="list-disc ps-5 text-gray-600">
            <li>Docker & Docker Compose</li>
            <li>CI/CD Pipelines (GitHub Actions)</li>
            <li>Linux Server Management</li>
            <li>Nginx / Apache</li>
            <li>Git & Code Reviews</li>
          </ul>
        </div>

        <div>
          <h3 class="text-lg font-semibold text-gray-500 mb-2">Backend Concepts</h3>
          <ul class="list-disc ps-5 text-gray-600">
            <li>REST API Design</li>
            <li>Authentication & Authorization (JWT, OAuth)</li>
            <li>Database Design & Migrations</li>
            <li>Caching (Redis)</li>
            <li>Background Jobs & Queues</li>
          </ul>
        </div>
        <div>
          <h3 class="text-lg font-semibold text-gray-500 mb-2">Testing</h3>
          <ul class="list-disc ps-5 text-gray-600">
            <li>Unit Testing</li>
            <li>API Testing (Postman)</li>
            <li>Basic E2E Testing</li>
            <li>Browser Testing (Playwright)</li>
          </ul>
        </div>
        <div>
          <h3 class="text-lg font-semibold text-gray-500 mb-2">Other Skills</h3>
          <ul class="list-disc ps-5 text-gray-600">
            <li>Problem Solving & Debugging</li>
            <li>Agile / Scrum Methodology</li>
            <li>Code Review & Refactoring</li>
            <li>Technical Documentation</li>
            <li>Cross-team Communication</li>
          </ul>
        </div>
        <div>
          <h3 class="text-lg font-semibold text-gray-500 mb-2">Languages</h3>
          <ul class="list-disc ps-5 text-gray-600">
            <li>English</li>
            <li>Arabic (fluent)</li>
            <li>German (basic)</li>
          </ul>
        </div>
      </div>
    </section>
    <div class="flex flex-col gap-2 md:gap-0 md:flex-row items-center md:justify-evenly w-full">
      <!-- Email -->
      <a href="mailto:mahmoud.elsayed.eg.1993@gmail.com"
        class="flex items-center gap-2 text-gray-300 hover:text-white transition">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
          <path
            d="M2.94 4.5A2.5 2.5 0 005.44 3h9.12a2.5 2.5 0 012.5 1.5L10 9 2.94 4.5zM18 7.05L10.16 12.4a.75.75 0 01-.32.1.75.75 0 01-.32-.1L2 7.05V14.5A2.5 2.5 0 004.5 17h11a2.5 2.5 0 002.5-2.5V7.05z" />
        </svg>
        <span>mahmoud.elsayed.eg.1993@gmail.com</span>
      </a>

      <!-- LinkedIn -->
      <a href="https://www.linkedin.com/in/mahmoud-elsayed-a03703212/" target="_blank" rel="noopener noreferrer"
        class="flex items-center gap-2 text-gray-300 hover:text-white transition">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24" fill="currentColor">
          <path
            d="M20.447 20.452h-3.749v-5.567c0-1.328-.025-3.038-1.849-3.038-1.851 0-2.135 1.445-2.135 2.94v5.665H9.064V9h3.6v1.561h.051c.5-.947 1.719-1.947 3.536-1.947 3.785 0 4.481 2.492 4.481 5.725v6.113zM5.337 7.433a2.167 2.167 0 110-4.333 2.167 2.167 0 010 4.333zM6.853 20.452H3.813V9h3.04v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.725v20.548C0 23.226.792 24 1.771 24h20.451c.98 0 1.771-.774 1.771-1.727V1.725C24 .774 23.205 0 22.225 0z" />
        </svg>
        <span>LinkedIn</span>
      </a>

      <!-- Github -->
      <a href="https://github.com/MahmoudElsayed-eg" target="_blank" rel="noopener noreferrer"
        class="flex items-center gap-2 text-gray-300 hover:text-white transition">
        <svg viewBox="0 0 24 24" aria-hidden="true" class="h-5 w-5" fill="currentColor">
          <path fill-rule="evenodd" clip-rule="evenodd"
            d="M12 2C6.477 2 2 6.463 2 11.97c0 4.404 2.865 8.14 6.839 9.458.5.092.682-.216.682-.48 0-.236-.008-.864-.013-1.695-2.782.602-3.369-1.337-3.369-1.337-.454-1.151-1.11-1.458-1.11-1.458-.908-.618.069-.606.069-.606 1.003.07 1.531 1.027 1.531 1.027.892 1.524 2.341 1.084 2.91.828.092-.643.35-1.083.636-1.332-2.22-.251-4.555-1.107-4.555-4.927 0-1.088.39-1.979 1.029-2.675-.103-.252-.446-1.266.098-2.638 0 0 .84-.268 2.75 1.022A9.607 9.607 0 0 1 12 6.82c.85.004 1.705.114 2.504.336 1.909-1.29 2.747-1.022 2.747-1.022.546 1.372.202 2.386.1 2.638.64.696 1.028 1.587 1.028 2.675 0 3.83-2.339 4.673-4.566 4.92.359.307.678.915.678 1.846 0 1.332-.012 2.407-.012 2.734 0 .267.18.577.688.48 3.97-1.32 6.833-5.054 6.833-9.458C22 6.463 17.522 2 12 2Z">
          </path>
        </svg>
        <span>Github</span>
      </a>
    </div>
  </main>
</template>
