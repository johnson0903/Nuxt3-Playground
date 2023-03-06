<script setup>
const runtimeConfig = useRuntimeConfig();
const appConfig = useAppConfig();

onMounted(() => {
  setTimeout(() => {
    appConfig.theme.dark = false;
    runtimeConfig.public.apiBase = "public path new";
  }, 3000);
});
function toggleTheme() {
  appConfig.theme.dark = !appConfig.theme.dark;
}
</script>
<template>
  <div>
    <h1>Nuxt config 檔案範例</h1>
    <div class="section">
      <h2>nuxt.config.ts</h2>
      <pre>runtime config api path: {{ runtimeConfig.public.apiBase }}</pre>
    </div>
    <div class="section">
      <h2>app.config.ts</h2>
      <p>app config 無法用 env file 覆寫</p>
      <pre>{{ appConfig }}</pre>
      <div class="theme-demo" :class="{ dark: appConfig.theme.dark }"></div>
      <button @click="toggleTheme">toggle theme</button>
      <NuxtLink to="/NuxtConfig2">NuxtConfig2 Page</NuxtLink>
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
