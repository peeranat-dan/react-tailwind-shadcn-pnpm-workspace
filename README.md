# React + Tailwind + Shadcn + pnpm-workspace

This is a [React](https://react.dev/) + [Tailwind](https://tailwindcss.com/) + [Shadcn](https://ui.shadcn.com/) + [pnpm-workspace](https://pnpm.io/workspaces) project.

## Project Structure

This monorepo contains:

- `apps/web` - React application with Vite
- `libs/ui` - Shared UI components library with Shadcn components
- `libs/tsconfig` - Shared TypeScript configuration

## Prerequisites

- [Node.js](https://nodejs.org/) (version 22.18 or higher)
- [pnpm](https://pnpm.io/) (version 10.12.1 or higher)

## Installation

1. Clone the repository:

```bash
git clone --depth=1 https://github.com/peeranat-dan/react-tailwind-pnpm-workspace.git
cd react-tailwind-pnpm-workspace
```

2. Install dependencies:

```bash
pnpm install
```

## Running the Project

### Development Mode

Start all applications and watch for changes:

```bash
pnpm dev
```

This will start:

- Web app at `http://localhost:5173`
- UI library CSS compilation in watch mode

### Individual Commands

Start only the web application:

```bash
cd apps/web
pnpm dev
```

Build the UI library:

```bash
cd libs/ui
pnpm build
```

### Building for Production

Build the web application:

```bash
cd apps/web
pnpm build
```

Preview the production build:

```bash
cd apps/web
pnpm preview
```

## Available Scripts

- `pnpm dev` - Start all packages in development mode
- `pnpm lint` - Run linting across the workspace
- `pnpm build` - Build all packages
