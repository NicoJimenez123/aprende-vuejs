<template>
  <p :class="'titulo ' + tituloClass">{{ titulo }}</p>
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  titulo: String,
  tituloClass: {
    type: String,
  },
})
</script>

<style scoped>
.titulo {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 1rem;
}
</style>
