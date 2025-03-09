<template>
  <div>
    <h1>Fundamentos de Programación: Variables</h1>
    <input v-model="variable" placeholder="Escribe algo..." />
    <p>Valor de la variable: {{ variable }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const variable = ref('')
</script>

<style scoped>
h1 {
  color: #333;
}

input {
  margin-top: 10px;
  padding: 5px;
  font-size: 16px;
}

p {
  margin-top: 10px;
  font-size: 18px;
}
</style>
