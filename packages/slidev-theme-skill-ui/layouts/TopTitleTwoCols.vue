<template>
  <div class="slidev-layout top-title-two-cols">
    <div class="slide-title">
      <slot name="title" />
    </div>
    <div class="columns-container">
      <div class="left-column">
        <slot name="left" />
      </div>
      <div class="right-column">
        <slot name="right" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.top-title-two-cols {
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

.columns-container {
  display: flex;
  gap: var(--spacing-xl);
  flex: 1;
}

.left-column,
.right-column {
  flex: 1;
  font-size: var(--font-size-body);
  line-height: var(--line-height-relaxed);
}
</style>