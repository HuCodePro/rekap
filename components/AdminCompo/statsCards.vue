<script setup>

defineProps({
  title: { type: String, default: 'Stat Title' },
  value: { type: [String, Number], default: '0' },
  description: { type: String, default: '' },
});
</script>

<template>
  <div class="stats shadow">
    <div class="stat">
      <div class="stat-title">{{ title }}</div>
      <div class="stat-value">{{ value }}</div>
      <div class="stat-desc">{{ description }}</div>
    </div>
  </div>
</template>

<style scoped>
.stats {
  transition: all 0.3s ease-in-out;
}
</style>
