<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        
        <q-toolbar-title> Carta de Presentación Antuanet </q-toolbar-title>

        <div>Quasar v{{ $q.version }}</div>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup>
// Ya que eliminamos el menú lateral (q-drawer), el bloque <script setup> 
// se vuelve mucho más simple, sin variables de estado (ref) ni funciones (toggle).

// Si quieres eliminar la advertencia de 'ref' no usado (si la tienes):
// import { ref } from 'vue' 
// Y quita la variable 'leftDrawerOpen' si la habías mantenido.

// Dejamos el script lo más limpio posible:

// Ya no necesitamos ninguna de las importaciones o variables que controlaban el menú lateral:
// import { ref } from 'vue'
// const leftDrawerOpen = ref(false)
// function toggleLeftDrawer() { leftDrawerOpen.value = !leftDrawerOpen.value }
</script>

<style scoped>
/* Sin estilos adicionales */
</style>