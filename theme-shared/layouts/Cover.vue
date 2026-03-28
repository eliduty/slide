<template>
  <div class="cover-layout">
    <div class="cover-content">
      <slot />
    </div>
    <div class="cover-footer">
      <slot name="footer" />
    </div>
  </div>
</template>

<style scoped>
.cover-layout {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  padding: 4rem;
}

.cover-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.cover-footer {
  padding-top: 2rem;
  font-size: 0.9rem;
  opacity: 0.7;
}
</style>