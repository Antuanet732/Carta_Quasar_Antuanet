<template>
<q-page padding class="row justify-center">
    <q-card class="q-pa-lg shadow-2 carta-container">
      
      <CartaEncabezado
        :nombre="datosCarta.nombre"
        :titulo="datosCarta.titulo"
        :email="datosCarta.email"
        :telefono="datosCarta.telefono"
      />

      <CartaDestinatario
        :destinatario="datosCarta.destinatario"
        :cargo="datosCarta.cargoDestinatario"
        :empresa="datosCarta.empresaDestinatario"
        :fecha="datosCarta.fecha"
      />

      <CartaCuerpo
        :introduccion="datosCarta.contenido.introduccion"
        :parrafo-principal="datosCarta.contenido.parrafoPrincipal"
        :cierre="datosCarta.contenido.cierre"
      />

      <CartaFirma
        :saludo="datosCarta.firma.saludo"
        :nombre-firma="datosCarta.firma.nombreFirma"
      />
      
    </q-card>
  </q-page>
</template>

<script setup>
// 1. IMPORTACIONES DE COMPONENTES
import CartaDestinatario from 'src/components/CartaDestinatario.vue';
import CartaEncabezado from 'src/components/CartaEncabezado.vue';
import CartaCuerpo from 'src/components/CartaCuerpo.vue';
import CartaFirma from 'src/components/CartaFirma.vue';

// 2. DECLARACIÓN DE LOS DATOS DE LA CARTA
const datosCarta = {
  nombre: 'Antuanet Web',
  titulo: 'Desarrolladora Vue.js & Quasar',
  email: 'antuanet.web@ejemplo.com',
  telefono: '+51 987 654 321',
  
  destinatario: 'Gerente de Contratación',
  cargoDestinatario: 'Departamento de Recursos Humanos',
  empresaDestinatario: 'TecnoCorp S.A.',
  fecha: new Date().toLocaleDateString('es-ES', { year: 'numeric', month: 'long', day: 'numeric' }),

  firma: {
    saludo: 'Agradezco sinceramente su tiempo y atención. Atentamente,',
    nombreFirma: 'Antuanet Web',
  },

  contenido: {
    introduccion: 'Escribo para expresar mi gran interés en la posición de Desarrolladora Frontend, como se anunció recientemente en LinkedIn.',
    parrafoPrincipal: 'Mi experiencia de 3 años en el desarrollo con Vue.js, complementada con el uso de Quasar Framework, me permite crear aplicaciones robustas, multiplataforma y con un diseño adaptable a cualquier dispositivo.',
    cierre: 'Estoy disponible para una entrevista en cualquier momento oportuno.'
  }
};
</script>
<style scoped>
/* Si quieres que la carta no ocupe todo el ancho, puedes añadir esto */
.carta-container {
  max-width: 800px;
  width: 100%;
}
</style>