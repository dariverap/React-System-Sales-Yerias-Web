# 🛠️ Ferreteria Yerias - Cliente Web

![React](https://img.shields.io/badge/react-%2320232a.svg?style=flat-square&logo=react&logoColor=%2361DAFB)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white)
![MUI](https://img.shields.io/badge/MUI-%230081CB.svg?style=flat-square&logo=mui&logoColor=white)
![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=flat-square&logo=bootstrap&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)

> Una Single Page Application (SPA) robusta para la gestión de operaciones de ferretería, incluyendo ventas, inventario, compras y gestión de proveedores.

---

### 🇺🇸 English Version: [Read here](./README.md)

---

## 🔗 Ecosistema y Repositorios Relacionados

Este repositorio es parte del **Ecosistema Ferreteria Yerias**. Asegúrate de tener la API backend en ejecución para una funcionalidad completa.

*   **Backend API (.NET):** [Net5-System-Sales-Yerias-RestAPI](https://github.com/dariverap/Net5-System-Sales-Yerias-RestAPI)

---

## 👨‍💻 Autor

**Creado por Diego Rivera**

---

## 💻 Tech Stack

Este proyecto está construido utilizando tecnologías frontend modernas para asegurar rendimiento y escalabilidad:

*   **Framework:** [React 18](https://reactjs.org/)
*   **Lenguaje:** [TypeScript](https://www.typescriptlang.org/)
*   **Estilos y UI:**
    *   [Material UI (MUI)](https://mui.com/) - Librería de componentes principal.
    *   [Bootstrap 5](https://getbootstrap.com/) - Layout y clases de utilidad.
    *   Styled Components.
*   **Peticiones de Datos:** [Axios](https://axios-http.com/)
*   **Visualización de Datos:** `@mui/x-data-grid` para tablas avanzadas.
*   **Utilidades:**
    *   `sweetalert2` para alertas modales.
    *   `pdf-lib` para generación de facturas y reportes en PDF.
    *   `dayjs` para manipulación de fechas.
    *   `formik` y `yup` para validación de formularios.

## 🏗️ Arquitectura

Este **Cliente Web** actúa como la capa de interfaz de usuario del ecosistema.

1.  **Comunicación:** Consume los endpoints de la API RESTful proporcionados por el servicio Backend.
2.  **Autenticación:** Implementa control de acceso basado en roles (Administrador, Vendedor, Almacenero) usando Cookies y LocalStorage.
3.  **Módulos:**
    *   **Catálogo:** Navegación y gestión de productos.
    *   **Ventas:** Interfaz de Punto de Venta (POS) con gestión de carrito.
    *   **Compras:** Gestión de la cadena de suministro y reabastecimiento.
    *   **Reportes:** Reportes de ventas e inventario.

## 🚀 Instalación y Configuración

### Prerrequisitos
*   Node.js (v16 o superior)
*   npm o yarn

### Pasos

1.  **Clonar el repositorio**
    ```bash
    git clone https://github.com/dariverap/React-System-Sales-Yerias-Web
    cd React-System-Sales-Yerias-Web
    ```

2.  **Instalar dependencias**
    ```bash
    npm install
    ```

3.  **Configuración de Entorno**
    Asegúrate de que la API esté corriendo. Por defecto, la aplicación busca la API en `https://localhost:44318/api-ferreteria/`.
    *Para cambiar esto, actualiza las URLs base en los archivos de servicio de los componentes.*

4.  **Ejecutar la aplicación**
    ```bash
    npm start
    ```
    La aplicación se abrirá en `http://localhost:3000`.

## 📦 Build para Producción

Para crear una compilación optimizada para producción:

```bash
npm run build
```