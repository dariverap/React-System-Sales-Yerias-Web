# 🛠️ Ferreteria Yerias - Web Client

![React](https://img.shields.io/badge/react-%2320232a.svg?style=flat-square&logo=react&logoColor=%2361DAFB)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white)
![MUI](https://img.shields.io/badge/MUI-%230081CB.svg?style=flat-square&logo=mui&logoColor=white)
![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=flat-square&logo=bootstrap&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)

> A robust Single Page Application (SPA) for managing hardware store operations, including sales, inventory, purchases, and supplier management.

---

### 🇪🇸 Versión en Español: [Leer aquí](./README.es.md)

---

## 🔗 Ecosystem & Related Repositories

This repository is part of the **Ferreteria Yerias Ecosystem**. Ensure you have the backend API running for full functionality.

*   **Backend API (.NET):** [Net5-System-Sales-Yerias-RestAPI](https://github.com/dariverap/Net5-System-Sales-Yerias-RestAPI)

---

## 👨‍💻 Author

**Created by Diego Rivera**

---

## 💻 Tech Stack

This project is built using modern frontend technologies to ensure performance and scalability:

*   **Framework:** [React 18](https://reactjs.org/)
*   **Language:** [TypeScript](https://www.typescriptlang.org/)
*   **Styling & UI:**
    *   [Material UI (MUI)](https://mui.com/) - Core component library.
    *   [Bootstrap 5](https://getbootstrap.com/) - Layout and utility classes.
    *   Styled Components.
*   **Data Fetching:** [Axios](https://axios-http.com/)
*   **Data Visualization:** `@mui/x-data-grid` for advanced tables.
*   **Utilities:**
    *   `sweetalert2` for modal alerts.
    *   `pdf-lib` for generating PDF invoices and reports.
    *   `dayjs` for date manipulation.
    *   `formik` & `yup` for form validation.

## 🏗️ Architecture

This **Web Client** acts as the user interface layer of the ecosystem.

1.  **Communication:** It consumes the RESTful API endpoints provided by the Backend service.
2.  **Authentication:** Implements role-based access control (Admin, Seller, Warehouse) using Cookies and LocalStorage.
3.  **Modules:**
    *   **Catalog:** Product browsing and management.
    *   **Sales:** Point of Sale (POS) interface with cart management.
    *   **Purchases:** Supply chain management and restocking.
    *   **Reports:** Sales and inventory reporting.

## 🚀 Installation & Setup

### Prerequisites
*   Node.js (v16 or higher)
*   npm or yarn

### Steps

1.  **Clone the repository**
    ```bash
    git clone https://github.com/dariverap/React-System-Sales-Yerias-Web
    cd React-System-Sales-Yerias-Web
    ```

2.  **Install dependencies**
    ```bash
    npm install
    ```

3.  **Environment Configuration**
    Ensure the API is running. By default, the app looks for the API at `https://localhost:44318/api-ferreteria/`.
    *To change this, update the base URLs in the component service files or refactor to use a `.env` file.*

4.  **Run the application**
    ```bash
    npm start
    ```
    The app will open at `http://localhost:3000`.

## 📦 Build for Production

To create an optimized production build:

```bash
npm run build
```