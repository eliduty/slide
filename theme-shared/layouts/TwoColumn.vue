<template>
  <div class="two-column-layout">
    <div class="left-column">
      <slot name="left" />
    </div>
    <div class="right-column">
      <slot name="right" />
    </div>
  </div>
</template>

<style scoped>
.two-column-layout {
  display: flex;
  gap: 2rem;
  height: 100%;
  padding: 2rem;
}

.left-column,
.right-column {
  flex: 1;
  display: flex;
  flex-direction: column;
}
</style>