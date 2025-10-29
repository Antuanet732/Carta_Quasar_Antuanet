# 📄 Carta de Presentación en Quasar & Vue 3

Este proyecto contiene una carta de presentación completamente desarrollada utilizando el framework Quasar (Vue 3) y la arquitectura basada en componentes, según lo solicitado.

---

## 🏗️ Arquitectura de Componentes

La aplicación sigue el principio de desarrollo modular de Vue.js. La carta se ha descompuesto y ensamblado utilizando los siguientes componentes re-utilizables que se encuentran en `src/components/`:

| Componente | Función Principal | Props Recibidas (Ejemplo) |
| :--- | :--- | :--- |
| `CartaEncabezado.vue` | Muestra los datos de contacto del remitente. | `nombre`, `titulo`, `email` |
| `CartaDestinatario.vue` | Muestra la información de la empresa y del contacto. | `empresa`, `destinatario` |
| `CartaCuerpo.vue` | Contiene los párrafos principales del mensaje. | `introduccion`, `párrafo1`, `párrafo2` |
| `CartaFirma.vue` | Muestra el saludo de cierre y la firma. | `saludo`, `nombreFirma` |

El ensamblaje final de la carta se realiza en la página principal: `src/pages/IndexPage.vue`.

---

## 🚀 Inicio del Proyecto

Para clonar y ejecutar este proyecto localmente:

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/Antuanet732/Carta_Quasar_Antuanet.git](https://github.com/Antuanet732/Carta_Quasar_Antuanet.git)
    ```
2.  **Entrar a la carpeta e instalar dependencias:**
    ```bash
    cd Carta_Quasar_Antuanet
    npm install
    ```
3.  **Ejecutar en modo desarrollo:**
    ```bash
    npm run dev
    ```

El proyecto se abrirá automáticamente en tu navegador (generalmente en `http://localhost:8080` o similar).

---
*(Tu Nombre Completo)*
See [Configuring quasar.config.js](https://v2.quasar.dev/quasar-cli-vite/quasar-config-js).
