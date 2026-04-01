# OpenRouter Project

A modern, full-stack web application built with TypeScript, React, and Elysia, demonstrating monorepo architecture using Turborepo. This project provides a scalable foundation for building web applications with multiple frontends and backends sharing common utilities.

## Author

- **GitHub**: [@lakshyaaa76](https://github.com/lakshyaaa76)
- **Email**: colossalmonk@gmail.com

## 🚀 Project Overview

OpenRouter is a comprehensive web application platform featuring:
- **Dashboard Frontend**: Modern React-based user interface with Tailwind CSS
- **API Backend**: RESTful API built with Elysia framework
- **Primary Backend**: Core backend services
- **Shared Database**: PostgreSQL with Prisma ORM for data management

## 🛠️ Tech Stack

### Frontend
- **React 19** - Modern React with latest features
- **TypeScript** - Type-safe JavaScript
- **Tailwind CSS** - Utility-first CSS framework
- **React Router v7** - Client-side routing
- **TanStack Query** - Server state management
- **Radix UI** - Accessible component primitives
- **Lucide React** - Beautiful icons

### Backend
- **Elysia** - Modern, fast web framework for Bun
- **TypeScript** - Type-safe backend development
- **Prisma** - Next-generation ORM
- **PostgreSQL** - Robust relational database

### Development Tools
- **Turborepo** - High-performance build system for monorepos
- **Bun** - Fast JavaScript runtime and package manager
- **ESLint** - Code linting and formatting
- **Prettier** - Code formatting

## 📁 Project Structure

```
openrouter/
├── apps/
│   ├── dashboard-frontend/    # React frontend application
│   ├── api-backend/          # Elysia API backend
│   └── primary-backend/      # Core backend services
├── packages/
│   └── db/                   # Shared database schema and utilities
├── turbo.json               # Turborepo configuration
└── package.json             # Root package configuration
```

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v18 or higher)
- **Bun** (v1.3.10 or higher)
- **PostgreSQL** (for database)
- **Git** (for version control)

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/lakshyaaa76/openrouter.git
cd openrouter
```

### 2. Install Dependencies

Using Bun (recommended):

```bash
bun install
```

Alternatively, using npm:

```bash
npm install
```

### 3. Environment Setup

Create a `.env` file in the root directory:

```env
# Database Configuration
DATABASE_URL="postgresql://username:password@localhost:5432/openrouter"

# Application Configuration
NODE_ENV="development"
PORT=3000
```

### 4. Database Setup

Run database migrations:

```bash
bun run db:migrate
```

Generate Prisma client:

```bash
bun run db:generate
```

## 🏃‍♂️ Development

### Start All Services

```bash
bun run dev
```

This will start:
- Dashboard Frontend: `http://localhost:3001`
- API Backend: `http://localhost:3000`
- Primary Backend: `http://localhost:3002`

### Individual Services

Start only the dashboard frontend:

```bash
cd apps/dashboard-frontend
bun run dev
```

Start only the API backend:

```bash
cd apps/api-backend
bun run dev
```

## 🔧 Available Scripts

- `bun run dev` - Start all applications in development mode
- `bun run build` - Build all applications for production
- `bun run lint` - Run ESLint across all packages
- `bun run format` - Format code with Prettier
- `bun run check-types` - Type check all TypeScript files

## 🏗️ Build & Deployment

### Build for Production

```bash
bun run build
```

### Deploy to Production

1. Build the application
2. Set up production environment variables
3. Deploy to your preferred hosting platform

## 📊 Features

- **Monorepo Architecture** - Organized codebase with shared packages
- **Type Safety** - Full TypeScript coverage across frontend and backend
- **Modern UI** - Responsive design with Tailwind CSS
- **API Integration** - RESTful APIs with Elysia
- **Database Management** - PostgreSQL with Prisma migrations
- **Developer Experience** - Hot reload, fast builds, and great tooling

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🔗 Useful Links

- [Turborepo Documentation](https://turborepo.dev/docs)
- [Elysia Documentation](https://elysiajs.com/)
- [React Documentation](https://react.dev/)
- [Prisma Documentation](https://www.prisma.io/docs/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
