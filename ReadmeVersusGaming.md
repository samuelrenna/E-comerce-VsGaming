# 🎮 Versus Gaming

**E-commerce desarrollado en React para productos de videojuegos.**

🔗 **[Ver Demo Desplegada en Vercel](https://proyecto-final-renna-l2ri.vercel.app/)**

---

## ⚠️ Estado del Proyecto (Base de Datos)
> **Atención:** La conexión con **Firebase** (Base de datos) se encuentra actualmente pausada debido a límites del plan gratuito.
> * **En el Deploy:** Es posible que los productos no carguen o el checkout no finalice.
> * **En Local:** Para probar la funcionalidad completa, necesitarás configurar tus propias credenciales (ver sección *Instalación*).

## 📋 Descripción
Versus Gaming es una Single Page Application (SPA) simulando una tienda en línea. Permite navegar por categorías, ver detalles de productos, gestionar un carrito de compras y simular un proceso de checkout.

## 🚀 Características Principales
* **Navegación Dinámica:** Rutas para Home, Categorías y Detalle de producto.
* **Gestión de Carrito:** Estado global manejado con Context API para agregar/eliminar items.
* **Checkout:** Formulario de compra validado para finalizar pedidos.
* **Feedback UI:** Notificaciones visuales para acciones del usuario usando `react-toastify`.
* **Diseño:** Interfaz responsiva con Bootstrap y CSS personalizado.

## 🛠️ Tecnologías Utilizadas
El proyecto utiliza las siguientes dependencias clave:
* **Core:** `React` (v18.2.0), `Vite`
* **Routing:** `react-router-dom` (v6.22.0)
* **Estilos:** `bootstrap` (v5.3.2), `react-bootstrap`
* **Backend (BaaS):** `firebase` (v10.8.1)
* **Utilidades:** `react-hook-form` (formularios), `react-toastify` (alertas)

## 📦 Instalación y Ejecución

Para ejecutar la aplicación localmente, sigue estos pasos:

1.  **Clona el repositorio:**
    ```bash
    git clone [https://github.com/tu-usuario/versus-gaming.git](https://github.com/tu-usuario/versus-gaming.git)
    cd versus-gaming
    ```

2.  **Instala las dependencias:**
    ```bash
    npm install
    ```

3.  **Configuración (Requerido para Base de Datos):**
    Para que la app funcione correctamente, debes crear un archivo `.env` en la raíz con tus propias credenciales de Firebase:
    ```env
    VITE_API_KEY=tu_api_key
    VITE_AUTH_DOMAIN=tu_proyecto.firebaseapp.com
    VITE_PROJECT_ID=tu_proyecto
    VITE_STORAGE_BUCKET=tu_proyecto.appspot.com
    VITE_MESSAGING_SENDER_ID=tu_sender_id
    VITE_APP_ID=tu_app_id
    ```

4.  **Ejecuta el servidor de desarrollo:**
    ```bash
    npm run dev
    ```

5.  **Abre tu navegador:**
    Ve a la dirección que te indique la terminal (usualmente `http://localhost:5173`) para ver la aplicación.

## 📂 Estructura del Proyecto

```text
versus-gaming/
│
├── public/              # Archivos estáticos
├── src/
│   ├── components/     # Componentes de React (NavBar, ItemList, Cart, etc.)
│   ├── context/        # Contexto global (CartContext)
│   ├── services/       # Configuración de Firebase
│   ├── styles/         # Archivos CSS
│   ├── App.jsx         # Componente principal y rutas
│   └── main.jsx        # Punto de entrada
│
├── .eslintrc.cjs       # Configuración de ESLint
├── index.html          # HTML principal
├── package.json        # Dependencias y scripts
└── vite.config.js      # Configuración de Vite