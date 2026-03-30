<template>
  <div class="slidev-layout section">
    <slot />
  </div>
</template>

<style scoped>
.section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  text-align: center;
  padding: var(--spacing-3xl);
}

.section :deep(h1) {
  font-size: var(--font-size-section-title);
  font-weight: 600;
  line-height: var(--line-height-tight);
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-md);
}

.section :deep(p) {
  font-size: var(--font-size-body);
  color: var(--color-text-secondary);
}
</style>