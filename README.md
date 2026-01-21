# Knowledge Index

An internal knowledge indexing and retrieval service demonstrating production-grade RAG pipelines, data boundaries, and AI reliability safeguards.

## Project Structure

This is a TypeScript monorepo using npm workspaces:

```
knowledge-index/
├── apps/
│   ├── frontend/          # React + TypeScript frontend
│   └── backend/           # Node + TypeScript API server
├── packages/
│   └── shared/            # Shared types and utilities
├── .eslintrc.json         # Root ESLint configuration
├── .prettierrc.json       # Prettier configuration
└── package.json           # Root workspace configuration
```

## Tech Stack

### Frontend

- **React 18** - UI framework
- **TypeScript** - Type safety
- **Vite** - Fast build tool and dev server
- **ESLint** - Code linting
- **Prettier** - Code formatting

### Backend

- **Node.js** - Runtime
- **Express** - Web framework
- **TypeScript** - Type safety
- **tsx** - TypeScript execution for development
- **ESLint** - Code linting
- **Prettier** - Code formatting

## Prerequisites

- Node.js >= 20.0.0
- npm >= 10.0.0

## Getting Started

### Installation

Install all dependencies for the monorepo:

```bash
npm install
```

### Development

Run all applications in development mode:

```bash
npm run dev
```

Or run applications individually:

```bash
# Frontend only (runs on http://localhost:3000)
npm run dev -w @knowledge-index/frontend

# Backend only (runs on http://localhost:3001)
npm run dev -w @knowledge-index/backend
```

### Building

Build all applications:

```bash
npm run build
```

Build specific workspace:

```bash
npm run build -w @knowledge-index/frontend
npm run build -w @knowledge-index/backend
```

### Linting

Run ESLint across all workspaces:

```bash
npm run lint
```

### Formatting

Format code with Prettier:

```bash
npm run format
```

Check formatting:

```bash
npm run format:check
```

### Type Checking

Run TypeScript type checking:

```bash
npm run type-check
```

## Workspace Commands

Run commands in specific workspaces using `-w` flag:

```bash
npm run <script> -w <workspace-name>
```

Examples:

```bash
npm run dev -w @knowledge-index/frontend
npm run lint -w @knowledge-index/backend
npm install <package> -w @knowledge-index/shared
```

## Environment Variables

### Backend

Copy the example environment file and configure as needed:

```bash
cp apps/backend/.env.example apps/backend/.env
```

## Project Conventions

- **Code Style**: Enforced by ESLint and Prettier
- **TypeScript**: Strict mode enabled across all packages
- **Naming**:
  - Components: PascalCase
  - Files: camelCase for utilities, PascalCase for components
  - Constants: UPPER_SNAKE_CASE
- **Imports**: Use absolute imports where configured

## License

Private - Internal use only
