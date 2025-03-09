<template>
  <div>
    <ElTitulo :titulo="'Fundamentos de Programación:'" />
    <p>1) Variables</p>
    <ElContenido>
      <template #contenido>
        <p v-html="contenido" />
      </template>
    </ElContenido>
  </div>
</template>

<script setup>
import ElTitulo from '@/components/ElTitulo.vue'
import ElContenido from '@/components/ElContenido.vue'

const contenido = `
  <p>Una variable es como una caja donde puedes guardar cosas. Imagina que tienes una caja con una etiqueta que dice "juguetes". Puedes poner cualquier juguete dentro de esa caja y cuando necesites un juguete, sabes exactamente dónde buscarlo. En programación, una variable funciona de manera similar: es un espacio en la memoria del computador donde puedes almacenar datos y luego acceder a ellos cuando los necesites.</p>
  <p>Por ejemplo (en Javascript):</p>
  <pre>
  <code>
  // Declarar una variable
  // Esto es como decirle al computador que tienes una caja llamada "caja"
  var caja

  // Asignar un valor a la variable
  // Aquí estamos poniendo un "juguete" dentro de la caja
  caja = "juguete"

  // Usar la variable
  // Ahora le decimos al computador que nos muestre lo que hay dentro de la caja
  console.log(caja); // Esto mostrará "juguete"
  </code>
  </pre>
`
</script>

<style>
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
