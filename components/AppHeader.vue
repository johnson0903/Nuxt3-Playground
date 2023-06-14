<template>
  <header>
    <ul class="nav">
      <li class="nav-item">
        <NuxtLink class="nav-link active" aria-current="page" to="/"
          >Home</NuxtLink
        >
      </li>
      <li class="nav-item">
        <NuxtLink class="nav-link" to="/NuxtConfig">Configuration</NuxtLink>
      </li>
      <li class="nav-item">
        <NuxtLink class="nav-link" to="/Assets">Assets</NuxtLink>
      </li>
      <li class="nav-item">
        <NuxtLink class="nav-link" to="/routing">Routing</NuxtLink>
      </li>
    </ul>
  </header>
</template>
<style scoped>
header {
  background-color: aquamarine;
}
</style>
