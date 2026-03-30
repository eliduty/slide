<template>
  <div class="slidev-layout top-title">
    <div class="slide-title">
      <slot name="title" />
    </div>
    <div class="slide-content">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.top-title {
  display: flex;
  flex-direction: column;
  height: 100%;
  padding: var(--spacing-2xl);
}

.slide-title {
  margin-bottom: var(--spacing-xl);
}

.slide-title :deep(h1) {
  font-size: var(--font-size-page-title);
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