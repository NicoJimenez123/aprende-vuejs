<template>
  <span :class="'contenido ' + contenidoClass">
    <slot name="contenido" />
  </span>
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  contenidoClass: {
    type: String,
    default: '',
  },
})
</script>

<style scoped>
.contenido {
  font-size: 18px;
  margin-top: 10px;
}
</style>
