<template>
  <div class="code-block">
    <div v-if="title" class="code-title">{{ title }}</div>
    <slot />
  </div>
</template>

<script setup>
defineProps({
  title: {
    type: String,
    default: ''
  }
})
</script>

<style scoped>
.code-block {
  margin: 1rem 0;
}

.code-title {
  font-size: 0.8rem;
  padding: 0.5rem 1rem;
  background: rgba(0, 0, 0, 0.1);
  border-radius: 4px 4px 0 0;
  margin-bottom: 0;
}
</style>