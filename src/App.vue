<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" /> -->
    <div class="flex justify-between flex-row-reverse  text-white p-6 max-w-5xl mx-auto">

      <div class="flex flex-row gap-2">
        <p @click="$i18n.locale = 'en'" class="cursor-pointer">en</p>
        <p @click="$i18n.locale = 'ar'" class="cursor-pointer">عربي</p>
      </div>
      <nav class="flex flex-row gap-2">
        <RouterLink class="" to="/">{{$t('home')}}</RouterLink>
        <!-- <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/test">Test</RouterLink> -->
      </nav>
    </div>
  </header>

  <RouterView />
</template>
