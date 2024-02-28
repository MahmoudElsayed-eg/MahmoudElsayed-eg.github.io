<script setup></script>

<template>
  <main :dir="$i18n.locale == 'ar' ? 'rtl' : 'ltr'">
    <h1>{{ $t('hello') }}</h1>
    <h2>{{ $t('job_title') }}</h2>
    <p>{{ $t('summary') }}</p>
    <p>{{ $t('projects') }}</p>
  </main>
</template>
