<script setup></script>

<template>
  <main
    :dir="$i18n.locale == 'ar' ? 'rtl' : 'ltr'"
    class="p-4 flex flex-col gap-3 items-center justify-center max-w-5xl mx-auto"
  >
    <h1 id="hello" class="mt-6 text-3xl font-semibold">{{ $t('hello') }}</h1>
    <h2 class="text-3xl font-semibold text-gray-400">{{ $t('job_title') }}</h2>
    <p class="text-gray-400">{{ $t('summary') }}</p>
    <a class="p-3 bg-green-900 rounded-lg" href="/Mahmoud_Elsayed.pdf" target="_blank">{{
      $t('cv')
    }}</a>
    <div class="p-6 rounded-lg shadow-lg w-full">
    <h2 class="text-2xl font-bold text-gray-400 mb-4">Skills</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <div>
        <h3 class="text-lg font-semibold text-gray-500 mb-2">Programming</h3>
        <ul class="list-disc pl-5 text-gray-600">
          <li>PHP</li>
          <li>Laravel</li>
          <li>Vue 3</li>
          <li>React</li>
          <li>Golang</li>
          <li>Kotlin</li>
          <li>SQL</li>
        </ul>
      </div>
      <div>
        <h3 class="text-lg font-semibold text-gray-500 mb-2">Frontend</h3>
        <ul class="list-disc pl-5 text-gray-600">
          <li>JavaScript</li>
          <li>HTML</li>
          <li>CSS</li>
          <li>Tailwind CSS</li>
        </ul>
      </div>
      <div>
        <h3 class="text-lg font-semibold text-gray-500 mb-2">Languages</h3>
        <ul class="list-disc pl-5 text-gray-600">
          <li>English</li>
          <li>Arabic (fluent)</li>
          <li>German (basic)</li>
        </ul>
      </div>
      <div>
        <h3 class="text-lg font-semibold text-gray-500 mb-2">Other Skills</h3>
        <ul class="list-disc pl-5 text-gray-600">
          <li>Problem Solving</li>
          <li>Communication</li>
          <li>Agile Development</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="flex flex-col items-center space-y-2">
      <!-- Email -->
      <a 
        href="mailto:mahmoud.elsayed.eg.1993@gmail.com" 
        class="flex items-center space-x-2 text-gray-300 hover:text-white transition">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
          <path d="M2.94 4.5A2.5 2.5 0 005.44 3h9.12a2.5 2.5 0 012.5 1.5L10 9 2.94 4.5zM18 7.05L10.16 12.4a.75.75 0 01-.32.1.75.75 0 01-.32-.1L2 7.05V14.5A2.5 2.5 0 004.5 17h11a2.5 2.5 0 002.5-2.5V7.05z" />
        </svg>
        <span>mahmoud.elsayed.eg.1993@gmail.com</span>
      </a>

      <!-- LinkedIn -->
      <a 
        href="https://www.linkedin.com/in/mahmoud-elsayed-a03703212/" 
        target="_blank" 
        rel="noopener noreferrer" 
        class="flex items-center space-x-2 text-gray-300 hover:text-white transition">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24" fill="currentColor">
          <path d="M20.447 20.452h-3.749v-5.567c0-1.328-.025-3.038-1.849-3.038-1.851 0-2.135 1.445-2.135 2.94v5.665H9.064V9h3.6v1.561h.051c.5-.947 1.719-1.947 3.536-1.947 3.785 0 4.481 2.492 4.481 5.725v6.113zM5.337 7.433a2.167 2.167 0 110-4.333 2.167 2.167 0 010 4.333zM6.853 20.452H3.813V9h3.04v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.725v20.548C0 23.226.792 24 1.771 24h20.451c.98 0 1.771-.774 1.771-1.727V1.725C24 .774 23.205 0 22.225 0z" />
        </svg>
        <span>LinkedIn</span>
      </a>
    </div>
  </main>
</template>
