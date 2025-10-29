<template>
  <q-card-section class="q-pt-md">
    <p class="text-body1 q-mb-sm">{{ saludo }}</p>
    <p class="text-h6 text-weight-bold">{{ nombreFirma }}</p>
  </q-card-section>
</template>

<script setup>
import { defineProps } from 'vue';

// CORRECCIÓN: Eliminamos 'const props ='
// El template accede a 'saludo' y 'nombreFirma' directamente.
defineProps({
  saludo: String,
  nombreFirma: String
});
</script>

<style scoped>
/* No se requiere CSS adicional, ya usamos Quasar */
</style>