<template>
  <main :dir="$i18n.locale == 'ar' ? 'rtl' : 'ltr'"
    class="p-4 flex flex-col gap-3 max-w-5xl mx-auto">
      <ProjectCard :title="$t('res_cms.title')" :desc="$t('res_cms.description')" :videos="['res_cms_admin.mp4','res_cms_main.mp4']" />
      <ProjectCard :title="$t('olive_cms.title')" :desc="$t('olive_cms.description')" :videos="['olive_cms.mp4']" />
  </main>
</template>
<script setup>
import ProjectCard from '@/components/ProjectCard.vue';
</script>
