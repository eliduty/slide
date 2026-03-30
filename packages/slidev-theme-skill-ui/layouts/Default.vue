<template>
  <div class="slidev-layout default">
    <slot />
  </div>
</template>

<style scoped>
.default {
  display: flex;
  flex-direction: column;
  height: 100%;
  padding: var(--spacing-2xl);
}

.default :deep(h1) {
  font-size: var(--font-size-page-title);
  font-weight: 600;
  line-height: var(--line-height-tight);
  margin-bottom: var(--spacing-xl);
  color: var(--color-text-primary);
}

.default :deep(h2) {
  font-size: var(--font-size-heading);
  font-weight: 600;
  line-height: var(--line-height-tight);
  margin-bottom: var(--spacing-lg);
  color: var(--color-text-primary);
}

.default :deep(ul),
.default :deep(ol) {
  font-size: var(--font-size-body);
  line-height: var(--line-height-relaxed);
}

.default :deep(li) {
  margin-bottom: var(--spacing-sm);
}
</style>