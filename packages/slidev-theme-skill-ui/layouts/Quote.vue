<template>
  <div class="slidev-layout quote">
    <slot />
  </div>
</template>

<style scoped>
.quote {
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100%;
  padding: var(--spacing-3xl);
}

.quote :deep(blockquote) {
  font-size: var(--font-size-heading);
  font-style: italic;
  line-height: var(--line-height-relaxed);
  margin: 0;
  padding-left: var(--spacing-lg);
  border-left: 4px solid var(--color-primary);
  color: var(--color-text-primary);
}

.quote :deep(cite) {
  display: block;
  margin-top: var(--spacing-lg);
  font-size: var(--font-size-body-sm);
  font-style: normal;
  color: var(--color-text-secondary);
}
</style>