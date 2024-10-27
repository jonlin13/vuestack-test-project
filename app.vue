<!-- app.vue -->
<template>
  <div class="container">
    <h1>VueStack Test Project</h1>
    <div class="build-info">
      <p>Build Time: {{ buildTime }}</p>
      <p>Environment: {{ environment }}</p>
    </div>
  </div>
</template>

<script setup>
const buildTime = new Date().toISOString()
const environment = process.env.NODE_ENV
</script>

<style>
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem;
  text-align: center;
}

.build-info {
  margin-top: 2rem;
  padding: 1rem;
  background: #f5f5f5;
  border-radius: 8px;
}
</style>
