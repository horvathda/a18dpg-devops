# Welcome to React Router!

A modern, production-ready template for building full-stack React applications using React Router.

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/remix-run/react-router-templates/tree/main/default)

## Features

- 🚀 Server-side rendering
- ⚡️ Hot Module Replacement (HMR)
- 📦 Asset bundling and optimization
- 🔄 Data loading and mutations
- 🔒 TypeScript by default
- 🎉 TailwindCSS for styling
- 📖 [React Router docs](https://reactrouter.com/)

## Getting Started

### Installation

Install the dependencies:

```bash
npm install
```

### Development

Start the development server with HMR:

```bash
npm run dev
```

Your application will be available at `http://localhost:5173`.

## Building for Production

Create a production build:

```bash
npm run build
```

## Deployment

### Docker Deployment

To build and run using Docker:

```bash
docker build -t my-app .

# Run the container
docker run -p 3000:3000 my-app
```

The containerized application can be deployed to any platform that supports Docker, including:

- AWS ECS
- Google Cloud Run
- Azure Container Apps
- Digital Ocean App Platform
- Fly.io
- Railway

### DIY Deployment

If you're familiar with deploying Node applications, the built-in app server is production-ready.

Make sure to deploy the output of `npm run build`

```
├── package.json
├── package-lock.json (or pnpm-lock.yaml, or bun.lockb)
├── build/
│   ├── client/    # Static assets
│   └── server/    # Server-side code
```

## Styling

This template comes with [Tailwind CSS](https://tailwindcss.com/) already configured for a simple default starting experience. You can use whatever CSS framework you prefer.

---

Built with ❤️ using React Router.

# a18dpg-devops

Ez a repo a DEVOPS tárgy beadandó projektfeladatához készült.  
A projekt egy egyszerű, „Hello world” szintű webes alkalmazás (Vite + React), amely HTTP-n érhető el, és tartalmazza a feladatban elvárt DevOps lépéseket:

- kódkészítés
- verziókövetés (Git, trunk-based jellegű használat)
- buildelés
- konténerizálás (Docker)
- kötelezően választandó rész: **Dev Container (VS Code / GitHub Codespaces)**

---

## 1. Alkalmazás

Az alkalmazás egy egyszerű frontend app, amely böngészőből érhető el HTTP-n keresztül, és egy „Hello world” jellegű oldalt jelenít meg.

Lokálisan (Docker nélkül) a fejlesztői szerver a következő címen érhető el:

- `http://localhost:5173`

---

## 2. Buildelés (kötelező rész)

A buildhez Node.js és npm szükséges.

### 2.1. Előfeltételek

- Node.js (ajánlott: aktuális LTS)
- npm
- Git

### 2.2. Lépések

```bash
git clone https://github.com/horvathda/a18dpg-devops.git
cd a18dpg-devops

# Függőségek telepítése
npm install

# Build
npm run build


# 3. Dev Container használata (kötelezően választható rész – opció 1)
   A projekt tartalmaz egy VS Code Dev Container konfigurációt a .devcontainer mappában, amely egy egységes, konténeres fejlesztői környezetet biztosít.

#3.1. Indítás VS Code-ban
   Előfeltételek:

   Docker Desktop (futó állapotban)

   Visual Studio Code

   Dev Containers bővítmény

#Lépések:

   Klónozd a repót:

   git clone https://github.com/horvathda/a18dpg-devops.git
   cd a18dpg-devops
   Nyisd meg a mappát Visual Studio Code-ban.

   A bal alsó sarokban kattints a duplanyíl ikonra, és válaszd a
   „Reopen in Container” opciót

   A konténer felépülése után futtasd:

   npm install
   npm run dev

´´´
```
