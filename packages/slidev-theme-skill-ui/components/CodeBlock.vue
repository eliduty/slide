<template>
  <div class="code-block">
    <div v-if="title" class="code-title">{{ title }}</div>
    <div class="code-content">
      <slot />
    </div>
  </div>
</template>

<script setup>
defineProps({
  title: {
    type: String,
    default: ''
  }
})
</script>

<style scoped>
.code-block {
  margin: var(--spacing-md) 0;
  border-radius: var(--radius-md);
  overflow: hidden;
  background-color: var(--color-bg-card);
  box-shadow: var(--shadow-xs);
}

.code-title {
  font-size: var(--font-size-caption);
  font-weight: 600;
  padding: var(--spacing-sm) var(--spacing-md);
  background: var(--color-bg-hover);
  color: var(--color-text-secondary);
  border-bottom: 1px solid var(--color-border);
}

.code-content {
  padding: var(--spacing-md);
  overflow-x: auto;
}

.code-content :deep(pre) {
  margin: 0;
  font-size: var(--font-size-code);
  font-family: var(--font-family-code);
  line-height: var(--line-height-normal);
}
</style>