cat > ~/Downloads/gymapp/README.md << 'EOF'
# 💪 Iron Gym App

Aplicación web multiplataforma para la gestión de un gimnasio de barrio.
Desarrollada como proyecto de portfolio del ciclo formativo DAM.

## 🚀 Demo en vivo
[Ver aplicación →](https://iron-gym-app.vercel.app)

## ✨ Funcionalidades

- 🔐 Login / Registro de usuarios (simulado)
- 📱 Código QR de acceso al gimnasio
- 📊 Dashboard con estadísticas de entrenamiento
- 📅 Reserva de clases grupales con disponibilidad en tiempo real
- 💾 Persistencia de reservas con localStorage
- 🏋️ Guía interactiva de máquinas con diagrama anatómico SVG
- 🌙 Modo oscuro / claro
- 📱 Diseño responsive (mobile-first)

## 🛠️ Tecnologías

- **React 18** — UI y gestión de estado
- **Vite** — Bundler y servidor de desarrollo
- **Context API + useReducer** — Estado global
- **localStorage** — Persistencia sin backend
- **SVG inline** — Diagramas anatómicos interactivos
- **CSS-in-JS** — Estilos con design tokens

## 🏗️ Arquitectura

src/
├── core/
│   ├── models/       → Entidades de negocio (User, GymClass)
│   └── services/     → Lógica desacoplada (AuthService, ClassService)
├── infrastructure/
│   └── mock/         → Datos simulados (reemplazable por API real)
├── state/            → Context + Reducers
├── features/         → Pantallas por dominio
│   ├── auth/
│   ├── dashboard/
│   ├── classes/
│   └── trainings/
└── shared/           → Componentes reutilizables


## 🔑 Credenciales de prueba

| Email | Contraseña | Plan |
|-------|-----------|------|
| alex@gym.com | gym123 | Premium |
| sara@gym.com | gym123 | Elite |
| marc@gym.com | gym123 | Basic |

## 👩‍💻 Autora

**Ana.is** — Estudiante DAM  
[LinkedIn](https://linkedin.com/in/ana-canton-gonzalez) · [GitHub](https://github.com/anacgonzalez97)

## 📄 Licencia

© 2025 Ana Bel. Todos los derechos reservados.  
Este proyecto es de uso personal y educativo.
EOF



# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
