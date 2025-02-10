# Health Terms Backend

[![TypeScript version][ts-badge]][typescript-5-7]
[![Node.js version][nodejs-badge]][nodejs]
[![APLv2][license-badge]][license]
[![Build Status - GitHub Actions][gha-badge]][gha-ci]

🏥 A robust backend service for managing and serving health-related terminology, built with TypeScript, Express, PostgreSQL, and Drizzle ORM.

## Features

- RESTful API endpoints for health terminology management
- PostgreSQL database integration for reliable data storage
- Type-safe database operations with Drizzle ORM
- Modern ESM-based architecture
- Comprehensive testing setup
- Production-ready configuration

## Tech Stack

- [TypeScript][typescript] [5.7][typescript-5-7]
- [Express.js](https://expressjs.com/) for API routing
- [PostgreSQL](https://www.postgresql.org/) for database
- [Drizzle ORM](https://orm.drizzle.team/) for database operations
- [ESM][esm] module system
- [ESLint][eslint] with health industry coding standards
- [Jest][jest] for unit testing and code coverage
- [Prettier][prettier] for consistent code style
- Type definitions for Node.js and Express
- [EditorConfig][editorconfig] for consistent coding style

## Getting Started

### Prerequisites

- Node.js (Latest LTS version)
- PostgreSQL installed and running
- bun or pnpm package manager

### Installation

1. Clone the repository:
```sh
git clone https://github.com/your-username/health-terms-backend
cd health-terms-backend
```

2. Install dependencies
```sh
bun install
```

3. Configure environment variables
open .env and edit these lines
```sh
APP_PORT=5000
NODE_ENV='development'
DATABASE_URL=postgresql://postgres:user@host:5432/database
```
4. Run database migrations:
```sh
bun run db:migrate
```

## Available Scripts

In the project directory, you can run:

### Database Scripts
- `bun db:ui` - Launch Drizzle Studio UI on port 3000 with verbose logging
- `bun db:generate` - Generate database migrations using Drizzle Kit
- `bun db:migrate` - Run database migrations
- `bun db:push` - Push database changes
- `bun db:seed` - Seed the database with initial data

### Development Scripts
- `bun start` - Run the production server from the dist folder
- `bun dev` - Start development server with hot reload using Bun
- `bun build` - Build the project using TypeScript compiler with alias support

### Testing Scripts
- `bun test` - Run unit tests using jest
- `bun test:watch` - Run tests in watch mode
- `bun test:coverage` - Run tests with coverage reporting

### Code Quality Scripts
- `bun lint` - Run ESLint to check code quality
- `bun prettier` - Format code using Prettier
- `bun prettier:check` - Check code formatting without making changes