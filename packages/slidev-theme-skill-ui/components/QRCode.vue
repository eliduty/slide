<template>
  <div class="qrcode-wrapper">
    <img v-if="dataUrl" :src="dataUrl" :alt="alt" :style="imgStyle" />
  </div>
</template>

<script setup>
import { ref, onMounted, computed } from 'vue'

const props = defineProps({
  value: {
    type: String,
    required: true
  },
  size: {
    type: Number,
    default: 200
  },
  alt: {
    type: String,
    default: 'QR Code'
  }
})

const dataUrl = ref('')

const imgStyle = computed(() => ({
  width: `${props.size}px`,
  height: `${props.size}px`
}))

onMounted(async () => {
  // 使用 QR Server API 生成二维码
  const encoded = encodeURIComponent(props.value)
  dataUrl.value = `https://api.qrserver.com/v1/create-qr-code/?size=${props.size}x${props.size}&data=${encoded}`
})
</script>

<style scoped>
.qrcode-wrapper {
  display: inline-block;
  padding: var(--spacing-sm);
  background-color: var(--color-bg-card);
  border-radius: var(--radius-md);
  box-shadow: var(--shadow-xs);
}

.qrcode-wrapper img {
  display: block;
  border-radius: var(--radius-sm);
}
</style>