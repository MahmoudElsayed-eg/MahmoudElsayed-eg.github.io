<template>
  <div>
    <button @click="$i18n.locale = 'en'" class="bg-white">en</button>
    <button @click="$i18n.locale = 'ar'">ar</button>
  </div>
  <h1>{{ $t('title') }}</h1>
</template>
<script setup></script>
