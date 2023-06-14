<template>
  <div class="section">
    <h2>public/ 資料夾</h2>
    <img src="/img/nuxt_logo.png" alt="Discover Nuxt 3" />
  </div>
  <div class="section">
    <h2>assets/ 資料夾</h2>
    <img src="~/assets/img/nuxt_logo_short.png" alt="Discover Nuxt 3" />
  </div>
  <div class="section">
    <h2>Global Styles imports</h2>
    <div class="global-style-primary"></div>
    <div class="global-style-secondary"></div>
  </div>
</template>
<style lang="scss">
.global-style-primary {
  width: 50px;
  height: 50px;
  background-color: $primary;
}
.global-style-secondary {
  width: 50px;
  height: 50px;
  background-color: $secondary;
}
</style>
