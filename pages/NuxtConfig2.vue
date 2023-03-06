<script setup>
const runtimeConfig = useRuntimeConfig();
const appConfig = useAppConfig();
</script>
<template>
  <div>
    <div class="section">
      <div class="theme-demo" :class="{ dark: appConfig.theme.dark }"></div>
      <NuxtLink to="/NuxtConfig">NuxtConfig Page</NuxtLink>
    </div>
  </div>
</template>
<style scoped>
.section {
  padding: 1rem;
  margin-bottom: 2rem;
  background-color: lightgray;
  border-radius: 8px;
}
.theme-demo {
  width: 100px;
  height: 100px;
  background-color: antiquewhite;
}
.theme-demo.dark {
  background-color: blueviolet;
}
</style>
