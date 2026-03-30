<template>
  <div class="slidev-layout two-cols">
    <div class="left-column">
      <slot name="left" />
    </div>
    <div class="right-column">
      <slot name="right" />
    </div>
  </div>
</template>

<style scoped>
.two-cols {
  display: flex;
  gap: var(--spacing-xl);
  height: 100%;
  padding: var(--spacing-2xl);
}

.left-column,
.right-column {
  flex: 1;
  display: flex;
  flex-direction: column;
  font-size: var(--font-size-body);
  line-height: var(--line-height-relaxed);
}
</style>