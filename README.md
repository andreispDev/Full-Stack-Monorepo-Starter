# Full Stack Monorepo Starter

A modern monorepo application built with **Astro**, **React**, **Express**, and **npm Workspaces**.

## Overview

This repository contains:

- **Web** - Public marketing website built with Astro
- **Client** - React application/dashboard
- **Server** - Express API backend
- **Shared** - Shared utilities, constants, validators, and reusable code

The project follows a scalable monorepo architecture suitable for small to medium-sized applications and enterprise internal systems.

---

## Tech Stack

### Frontend

- Astro
- React
- Vite
- Tailwind CSS

### Backend

- Express.js
- Node.js
- TypeScript

### Database

- MySQL

### Tooling

- npm Workspaces
- Prettier
- EditorConfig
- GitHub Actions

---

## Project Structure

```text
company-platform/
│
├── apps/
│   ├── web/              # Astro Website
│   ├── client/           # React Dashboard
│   └── server/           # Express API
│
├── packages/
│   └── shared/           # Shared Code
│
├── .github/
│   └── workflows/
│
├── .editorconfig
├── .env.example
├── .gitignore
├── .prettierignore
├── .prettierrc
├── .nvmrc
├── LICENSE
├── README.md
└── package.json
```

---

## Requirements

- Node.js 22+
- npm 10+
- MySQL 8+

---

## Installation

### Clone Repository

```bash
git clone <repository-url>
cd mono-repo
```

### Install Dependencies

```bash
npm install
```

### Configure Environment Variables

Copy the example environment file:

```bash
cp .env.example .env
```

Configure the values according to your environment.

---

## Running Applications

### Run Everything

```bash
npm run dev
```

### Run Individual Applications

#### Astro Website

```bash
npm run web
```

#### React Client

```bash
npm run client
```

#### Express Server

```bash
npm run server
```

---

## Development URLs

| Service | URL                   |
| ------- | --------------------- |
| Website | http://localhost:4321 |
| Client  | http://localhost:5173 |
| Server  | http://localhost:5000 |

---

## Shared Package

Reusable code can be placed inside:

```text
packages/shared/
```

Examples:

- Roles
- Permissions
- Validation Rules
- Utility Functions
- Constants

Example usage:

```javascript
import { ROLES } from "@company/shared";
```

---

## Code Formatting

Check formatting:

```bash
npm run format:check
```

Format code:

```bash
npm run format
```

---

## Build

### Website

```bash
npm run build --prefix apps/web
```

### Client

```bash
npm run build --prefix apps/client
```

### Server

```bash
npm run build --prefix apps/server
```

---

## Environment Variables

See:

```text
.env.example
```

for all available environment variables.

---

## GitHub Actions

CI workflow configuration:

```text
.github/workflows/ci.yml
```

The workflow automatically:

- Installs dependencies
- Checks formatting
- Builds applications
- Validates pull requests

---

## License

This project is licensed under the MIT License.

See the LICENSE file for details.

---

## Author

Andrei Portugal

Programmer | Full Stack Developer

---

## Future Improvements

- Authentication & Authorization (RBAC)
- Docker Support
- Swagger API Documentation
- Unit Testing
- Integration Testing
- CI/CD Deployment
- Shared UI Component Library
- Shared TypeScript Types
