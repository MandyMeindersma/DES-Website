<script setup lang="ts">
useServerSeoMeta({
  title: 'Dev Edmonton Society',
  titleTemplate: '%s | Dev Edmonton Society',
  description: 'Dev Edmonton Society is a community of developers, designers, and tech enthusiasts in Edmonton, Alberta.',
  author: 'Dev Edmonton Society',
  themeColor: '#265DAD',
})
</script>

<template>
  <Html>
    <Body class="bg-neutral-100 dark:bg-neutral-900 dark:text-white transition-all duration-300">
      <NuxtLoadingIndicator />
      <AppHeader />
      <NuxtPage />
      <AppFooter />
    </Body>
  </Html>
</template>
