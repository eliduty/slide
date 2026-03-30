<template>
  <span class="badge" :class="type">
    <slot />
  </span>
</template>

<script setup>
defineProps({
  type: {
    type: String,
    default: 'default',
    validator: (value) => ['default', 'primary', 'success', 'warning', 'error', 'info'].includes(value)
  }
})
</script>

<style scoped>
.badge {
  display: inline-flex;
  align-items: center;
  padding: 2px 8px;
  font-size: var(--font-size-caption);
  font-weight: 500;
  border-radius: var(--radius-sm);
  white-space: nowrap;
}

/* Default */
.badge.default {
  background-color: var(--color-bg-hover);
  color: var(--color-text-secondary);
}

/* Primary */
.badge.primary {
  background-color: var(--color-primary-light);
  color: var(--color-primary);
}

/* Success */
.badge.success {
  background-color: var(--color-success-light);
  color: var(--color-success);
}

/* Warning */
.badge.warning {
  background-color: var(--color-warning-light);
  color: var(--color-warning);
}

/* Error */
.badge.error {
  background-color: var(--color-error-light);
  color: var(--color-error);
}

/* Info */
.badge.info {
  background-color: var(--color-info-light);
  color: var(--color-info);
}
</style>