# Flux_full — Full-Stack Trading Platform with Next.js 15, Express 5 & MongoDB

A **full-stack trading platform web application** in a single repository: a **Next.js 15 / React 19** frontend built with **TypeScript, Tailwind CSS, and Radix UI**, backed by an **Express 5 + MongoDB (Mongoose)** REST API with **JWT authentication**.

The frontend is a modern, component-rich interface — full Radix UI primitive set, form handling with validation, charts, and dark-mode support. The backend (`trading-platform`) provides the API layer with hashed-password auth and token-based sessions.

## Features

### Frontend (`frontend/`)
- **Next.js 15 + React 19** with TypeScript
- **Radix UI components** throughout (dialogs, menus, tabs, selects, accordions, toasts, and more) with **Tailwind CSS 3** styling
- **Forms** with react-hook-form + Zod validation
- **Charts** with Recharts and date utilities via date-fns
- **Dark mode** support via next-themes; icons from lucide-react

### Backend (`backend/`)
- **Express 5** REST API (`server.js`)
- **MongoDB** data layer with **Mongoose 8**
- **JWT authentication** (jsonwebtoken) with **bcrypt** password hashing
- CORS enabled, environment-based configuration with dotenv
- Developer workflow with nodemon (`npm run dev`)

## Tech Stack

- **Frontend:** Next.js 15, React 19, TypeScript 5, Tailwind CSS 3, Radix UI, react-hook-form, Zod, Recharts
- **Backend:** Node.js, Express 5, MongoDB + Mongoose 8, JSON Web Tokens, bcrypt
- **Tooling:** npm, nodemon

## Project Structure

```
Flux_full/
├── frontend/      # Next.js 15 trading-platform UI (TypeScript)
├── backend/       # Express 5 + MongoDB API (JWT auth)
└── package.json   # Root package configuration
```

## Getting Started

Clone the repository:

```bash
git clone https://github.com/sh00von/Flux_full.git
cd Flux_full
```

### Run the backend

```bash
cd backend
npm install
# create a .env with your MongoDB connection string and JWT secret
npm run dev     # nodemon server.js
# or: npm start
```

### Run the frontend

```bash
cd frontend
npm install
npm run dev     # Next.js dev server on http://localhost:3000
npm run build   # production build
```

---

⭐ Star the repo if the structure is useful for your own full-stack TypeScript/JavaScript projects — contributions are welcome!
