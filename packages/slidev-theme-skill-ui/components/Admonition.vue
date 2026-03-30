<template>
  <div class="admonition" :class="type">
    <div class="admonition-icon">
      <span v-if="type === 'info'">ℹ️</span>
      <span v-else-if="type === 'warning'">⚠️</span>
      <span v-else-if="type === 'error'">❌</span>
      <span v-else-if="type === 'success'">✅</span>
    </div>
    <div class="admonition-content">
      <div v-if="title" class="admonition-title">{{ title }}</div>
      <slot />
    </div>
  </div>
</template>

<script setup>
defineProps({
  type: {
    type: String,
    default: 'info',
    validator: (value) => ['info', 'warning', 'error', 'success'].includes(value)
  },
  title: {
    type: String,
    default: ''
  }
})
</script>

<style scoped>
.admonition {
  display: flex;
  gap: var(--spacing-md);
  padding: var(--spacing-md);
  border-radius: var(--radius-md);
  margin: var(--spacing-md) 0;
  font-size: var(--font-size-body-sm);
}

.admonition-icon {
  flex-shrink: 0;
  font-size: 1.2em;
}

.admonition-content {
  flex: 1;
}

.admonition-title {
  font-weight: 600;
  margin-bottom: var(--spacing-xs);
}

/* Info */
.admonition.info {
  background-color: var(--color-info-light);
  border-left: 4px solid var(--color-info);
  color: var(--color-text-primary);
}

/* Warning */
.admonition.warning {
  background-color: var(--color-warning-light);
  border-left: 4px solid var(--color-warning);
  color: var(--color-text-primary);
}

/* Error */
.admonition.error {
  background-color: var(--color-error-light);
  border-left: 4px solid var(--color-error);
  color: var(--color-text-primary);
}

/* Success */
.admonition.success {
  background-color: var(--color-success-light);
  border-left: 4px solid var(--color-success);
  color: var(--color-text-primary);
}
</style>