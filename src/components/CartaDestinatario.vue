<template>
  <q-card-section class="q-pt-sm q-pb-md">
    <div class="text-subtitle2 text-weight-bold q-mb-xs">{{ destinatario }}</div>
    <div class="text-subtitle2 text-grey-8">{{ cargo }}</div>
    <div class="text-subtitle2 text-grey-8">{{ empresa }}</div>
    <div class="text-caption text-grey-6 q-mt-xs">{{ fecha }}</div>
  </q-card-section>
</template>

<script setup>
import { defineProps } from 'vue';

// Este componente recibirá 4 datos (props) desde el padre (IndexPage.vue)
const props = defineProps({
  destinatario: String,
  cargo: String,
  empresa: String,
  fecha: String
});
</script>

<style scoped>
/* No se requiere CSS adicional, ya usamos las clases de Quasar para el estilo */
</style>