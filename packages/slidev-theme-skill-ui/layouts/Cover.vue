<template>
  <div class="slidev-layout cover">
    <div class="cover-content">
      <slot />
    </div>
    <div class="cover-footer">
      <slot name="footer" />
    </div>
  </div>
</template>

<style scoped>
.cover {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  padding: var(--spacing-3xl);
}

.cover-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.cover-content :deep(h1) {
  font-size: var(--font-size-cover-title);
  font-weight: 600;
  line-height: var(--line-height-tight);
  margin-bottom: var(--spacing-md);
  color: var(--color-text-primary);
}

.cover-content :deep(p) {
  font-size: var(--font-size-cover-subtitle);
  color: var(--color-text-secondary);
  margin-bottom: var(--spacing-md);
}

.cover-footer {
  padding-top: var(--spacing-xl);
  font-size: var(--font-size-cover-meta);
  color: var(--color-text-secondary);
}
</style>