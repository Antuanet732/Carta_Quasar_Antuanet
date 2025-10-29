<template>
  <q-card-section class="q-pt-lg q-pb-none">
    
    <p class="text-body1 q-mb-md">
      {{ introduccion }}
    </p>

    <p class="text-body1 q-mb-lg">
      {{ parrafoPrincipal }}
    </p>

    <p class="text-body1 q-mb-xl">
      {{ cierre }}
    </p>

  </q-card-section>
</template>

<script setup>
import { defineProps } from 'vue';

// CORRECCIÓN: Eliminamos 'const props ='
// El template accede a 'introduccion', 'parrafoPrincipal', etc., directamente.
defineProps({
  introduccion: String,
  parrafoPrincipal: String,
  cierre: String
});
</script>

<style scoped>
/* No se requiere CSS adicional, ya usamos las clases de Quasar para el estilo */
</style>