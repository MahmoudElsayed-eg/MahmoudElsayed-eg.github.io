<template>
  <div>
    <button @click="$i18n.locale = 'en'" class="bg-white">en</button>
    <button @click="$i18n.locale = 'ar'">ar</button>
  </div>
  <h1>{{ $t('name') }}</h1>
  <p :dir="$i18n.locale == 'ar' ? 'rtl':'ltr'">{{ $t('summary') }}</p>
</template>
<script setup></script>
