<template>
  <div class="slidev-layout side-title">
    <div class="slide-title">
      <slot name="title" />
    </div>
    <div class="slide-content">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.side-title {
  display: flex;
  gap: var(--spacing-xl);
  height: 100%;
  padding: var(--spacing-2xl);
}

.slide-title {
  flex-shrink: 0;
  width: 30%;
  display: flex;
  align-items: flex-start;
  justify-content: center;
  flex-direction: column;
}

.slide-title :deep(h1) {
  font-size: var(--font-size-heading);
  font-weight: 600;
  line-height: var(--line-height-tight);
  color: var(--color-text-primary);
  margin: 0;
}

.slide-content {
  flex: 1;
  font-size: var(--font-size-body);
  line-height: var(--line-height-relaxed);
}
</style>