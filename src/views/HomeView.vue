<script setup></script>

<template>
  <main
    :dir="$i18n.locale == 'ar' ? 'rtl' : 'ltr'"
    class="p-4 flex flex-col gap-3 items-center justify-center max-w-5xl mx-auto"
  >
    <h1 class="mt-6 text-3xl font-semibold">{{ $t('hello') }}</h1>
    <h2 class="text-3xl font-semibold text-gray-400">{{ $t('job_title') }}</h2>
    <p class="text-gray-400">{{ $t('summary') }}</p>
    <a class="p-3 bg-green-900 rounded-lg" href="/Mahmoud Elsayed.pdf" target="_blank">{{
      $t('cv')
    }}</a>
    <div class="w-full mt-6 space-y-3">
      <p class="mt-6 text-3xl font-semibold">{{ $t('projects') }}</p>
      <a
        class="border border-gray-700 flex flex-col md:flex-row gap-2"
        href="https://cs.gomlamarket.com"
        target="_blank"
        rel="noopener noreferrer"
      >
        <div class="bg-white">
          <img src="/gm.png" class="w-40 h-40 mx-auto" alt="" />
        </div>
        <div class="p-5 space-y-3">
          <h2 class="font-medium text-xl">{{ $t('gm') }}</h2>
          <p class="text-gray-400">{{ $t('gm_desc') }}</p>
        </div>
      </a>
    </div>
  </main>
</template>
