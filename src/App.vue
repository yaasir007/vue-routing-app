<script setup>
import { RouterView, RouterLink } from 'vue-router' 
</script>

<template>
  <main>
    <div class="links">
      <RouterLink active-class="active" to="/">Home</RouterLink>
      <RouterLink active-class="active" to="/about">About</RouterLink>
    </div>
    <RouterView />
  </main>
</template>

<style scoped>
.links {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2rem;
}

.active {
  font-weight: bold;
  color: brown;
}
</style>