<template>
  <ul class="nav">
    <li class="nav-item">
      <NuxtLink
        class="nav-link active"
        aria-current="page"
        to="/routing/dashboard"
        >Dashboard</NuxtLink
      >
    </li>
    <li class="nav-item">
      <NuxtLink class="nav-link" to="/routing/posts/1">posts 1</NuxtLink>
    </li>
    <li class="nav-item">
      <NuxtLink class="nav-link" to="/routing/posts/2">posts 2</NuxtLink>
    </li>
  </ul>
</template>
