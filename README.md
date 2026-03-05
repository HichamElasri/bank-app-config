<p align="center">
  <br />
  <img src="./assets/e-bank-logo.png" width="400px" />
</p>
<div align="center">

[![React](https://img.shields.io/badge/React-^19.1.0-61dafb?logo=react&logoColor=white)](https://reactjs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-~5.8.3-3178c6?logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![Vite](https://img.shields.io/badge/Vite-^6.3.5-646cff?logo=vite&logoColor=white)](https://vitejs.dev)
[![React Query](https://img.shields.io/badge/React_Query-^5.76.1-ff4154?logo=reactquery&logoColor=white)](https://tanstack.com/query)
[![Redux Toolkit](https://img.shields.io/badge/Redux_Toolkit-^2.8.1-764abc?logo=redux&logoColor=white)](https://redux-toolkit.js.org)
[![React Router](https://img.shields.io/badge/React_Router-^7.6.0-ca4245?logo=reactrouter&logoColor=white)](https://reactrouter.com)
[![Material-UI](https://img.shields.io/badge/Material_UI-^7.1.0-007fff?logo=mui&logoColor=white)](https://mui.com)
[![React Hook Form](https://img.shields.io/badge/React_Hook_Form-^7.56.4-ec5990?logo=reacthookform&logoColor=white)](https://react-hook-form.com)
[![Zod](https://img.shields.io/badge/Zod-^3.25.76-3e67b1?logo=zod&logoColor=white)](https://zod.dev)
[![Axios](https://img.shields.io/badge/Axios-^1.9.0-5a29e4?logo=axios&logoColor=white)](https://axios-http.com)
[![ESLint](https://img.shields.io/badge/ESLint-^9.25.0-4b32c3?logo=eslint&logoColor=white)](https://eslint.org)
[![Prettier](https://img.shields.io/badge/Prettier-3.38.3-F7B93E?logo=prettier&logoColor=white)](https://prettier.io)
[![]()]()

</div>

## 📑 <a name="table">Table of Contents</a>

1. 📌 [About the project](#about-the-project)
2. 🎥 [Demo](#demo)
3. ✨ [Features](#features)
4. 🛠️ [Tech Stack](#tech-stack)
5. 📁 [Project Structure](#project-structure)
6. ⚡ [Quick Start](#quick-start)
7. 🤝 [Contributing](#contributing)
8. ✉️ [Contact](#contact)

## <a name="about-the-project">📌 About the project</a>

**E-Bank (Frontend)** is a React-based web application designed to manage bank customers, accounts and financial transactions. The application provides essential banking operations including depositing funds, making payment, transferring money between accounts and withdrawing funds.

## <a name="demo">🎥 Demo</a>

![E-Bank Demo](./assets/demo-e-bank-1.5_720.gif)
![E-Bank Demo](./assets/demo-e-bank-1.5.gif)

## <a name="features">✨ Features</a>

- JWT-based authentication and authorization for secure access control.
- Customer management with create, update and delete operations.
- Support for multiple bank accounts (Checking and Savings) per customer.
- Processing of financial transactions with balance validation and real-time updates, including:
  - Fund deposits.
  - Bill payments.
  - Internal account transfers.
  - Fund withdrawals.

## <a name="tech-stack">🛠️ Tech Stack</a>

- **React** ^19.1.0
- **TypeScript** ~5.8.3
- **Vite** ^6.3.5
- **React Query** ^5.76.1
- **Redux Toolkit** ^2.8.1
- **React Router** ^7.6.0
- **Material-UI** ^7.1.0
- **React Hook Form** ^7.56.4
- **Zod** ^3.25.76
- **Axios** ^1.9.0
- **ESLint** ^9.25.0
- **Prettier** ^3.38.3

## <a name="project-structure">📁 Project Structure</a>

Overview of the project structure, including the main folders and architectural layers:

```
e-bank-frontend/
├─ src/
│ ├─ assets/              # Static files (images, fonts, icons...)
│ ├─ components/          # Reusable UI components
│ │ ├─ common/            # Composite components
│ │ ├─ ui/                # Fundamental components
│ ├─ features/            # Feature modules
│ │ ├─ account/           # Account feature domain
│ │ │ ├─ adapters/        # Data adapters
│ │ │ ├─ components/      # Feature-specific components
│ │ │ ├─ config/          # Feature configuration
│ │ │ ├─ constants/       # Feature constants
│ │ │ ├─ hooks/           # Feature-specific custom hooks
│ │ │ ├─ pages/           # Feature pages
│ │ │ ├─ services/        # Feature services (API calls & data fetching)
│ │ │ ├─ types/           # Feature-specific TypeScript types (Types, DTOs, Enums...)
│ │ │ └─ validators/      # Validation schemas
│ │ ├─ auth/              # Authentication feature domain
│ │ ├─ customer/          # Customer feature domain
│ │ └─ transaction/       # Transaction feature domain
│ ├─ guards/              # Authentication & authorization guards
│ ├─ hooks/               # Global custom hooks
│ ├─ layouts/             # Layouts components
│ ├─ lib/                 # Utility libraries (axios, react-query...)
│ ├─ pages/               # Top-level page components
│ ├─ providers/           # Application providers
│ ├─ routes/              # Routing configuration
│ ├─ store/               # Global state store
│ ├─ styles/              # Global styles & themes
│ ├─ types/               # Global TypeScript types
│ ├─ utils/               # Utility functions & helpers
```

## <a name="quick-start">⚡ Quick Start</a>

Follow these steps to set up the project locally on your machine.

**Prerequisites**

Make sure you have the following installed on your machine:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)
- [E-Bank (Backend)](https://github.com)

**Cloning the Repository**

```bash
git clone https://github.com
cd e-bank-frontend
```

**Installation**

Install the project dependencies using npm:

```bash
npm install
```

**Set Up Environment Variables**

Create a new file named `.env` in the root of your project and add the following content:

```env
VITE_API_BASE_URL=http://localhost:9191/
VITE_AUTH_SERVICE_URL=realms/e-bank-dev/protocol/openid-connect
VITE_ACCOUNT_SERVICE_URL=account-service/v1/accounts
VITE_CUSTOMER_SERVICE_URL=customer-service/v1/customers
VITE_TRANSACTION_SERVICE_URL=transaction-service/v1/transactions
VITE_KEYCLOAK_CLIENT_ID=e-bank-api
VITE_KEYCLOAK_GRANT_TYPE=password
```

**Running the Project**

```bash
npm run dev
```

Once the development server is running, navigate to http://localhost:5173/auth/sign-in via your browser and authenticate using the credentials below:

| Role  | Username | Password |
| ----- | -------- | -------- |
| Admin | admin    | admin    |

## <a name="contributing">🤝 Contributing</a>

- If you find this project useful, please consider giving it a start ⭐. Thanks!
- Feel free to suggest improvements or report any issues in the repository.

## <a name="contact">✉️ Contact</a>

If you have any question or feedback, please feel free to contact me:

- **Maintainer**: ELASRI Hicham - [in/hichamelasri]() - `hi.elasri@gmail.com`
- **Project Link**: https://github.com/
