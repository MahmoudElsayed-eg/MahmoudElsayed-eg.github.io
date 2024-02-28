<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" /> -->
    <div class="flex justify-between flex-row-reverse">

      <div class="flex flex-row gap-2">
        <p @click="$i18n.locale = 'en'">en</p>
        <p @click="$i18n.locale = 'ar'">عربي</p>
      </div>
      <nav class="flex flex-row gap-2">
        <RouterLink class="" to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/test">Test</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
