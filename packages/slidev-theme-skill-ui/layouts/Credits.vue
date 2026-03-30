<template>
  <div class="slidev-layout credits">
    <slot />
  </div>
</template>

<style scoped>
.credits {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  text-align: center;
  padding: var(--spacing-3xl);
}

.credits :deep(h1) {
  font-size: var(--font-size-heading);
  font-weight: 600;
  color: var(--color-text-primary);
  margin-bottom: var(--spacing-lg);
}

.credits :deep(p) {
  font-size: var(--font-size-body);
  color: var(--color-text-secondary);
  margin-bottom: var(--spacing-md);
}

.credits :deep(a) {
  color: var(--color-primary);
}
</style>