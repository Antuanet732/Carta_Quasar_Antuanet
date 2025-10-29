<template>
  <q-card flat class="q-mb-lg">
    <q-card-section>
      <div class="text-h4 text-weight-bold">{{ nombre }}</div>
      <div class="text-subtitle1 text-grey-7">{{ titulo }}</div>
      
      <q-separator class="q-my-sm" /> 

      <div class="text-caption">
        <q-icon name="mail" size="xs" class="q-mr-xs" /> Email: {{ email }} 
        <span class="q-mx-md">|</span> 
        <q-icon name="phone" size="xs" class="q-mr-xs" /> Teléfono: {{ telefono }}
      </div>
    </q-card-section>
  </q-card>
</template>

<script setup>
import { defineProps } from 'vue';

// CORRECCIÓN: Quitamos 'const props =' ya que no se usa en este bloque
// El template puede acceder a 'nombre', 'titulo', etc., directamente.
defineProps({
  nombre: String,
  titulo: String,
  email: String,
  telefono: String
});
</script>

<style scoped>
/* No se requiere CSS adicional */
</style>