# Client API + Svelte + TS + Vite

A template for building WedStation client API applications using Svelte, TypeScript, and Vite. 

Intended to be installed on a Schneider Electric [EcoStruxure Building Operation](https://www.se.com/us/en/product-range/62111-ecostruxure-building-operation-software/#overview) and is accessed with [WebStation](https://ecostruxure-building-help.se.com/bms/topics/show.castle?id=8792&productversion=7.0&locale=en-US)

This project comes with built-in support for TailwindCSS, ESLint, and Prettier configuration.


## Features

- 🚀 [Svelte 5](https://svelte.dev/) with TypeScript
- ⚡️ [Vite 7](https://vitejs.dev/) for super-fast development
- 🎨 [TailwindCSS 4](https://tailwindcss.com/) for styling
- 📦 Single-file build option
- ✨ ESLint + Prettier for code quality
- 🔍 TypeScript strict mode enabled

## Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- npm or pnpm (recommended)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/tom-pacheco-bcm/client-template.git
cd client-template
```

2. Install dependencies:
```bash
npm install
# or with pnpm
pnpm install
```

## Development

To start the development server:

```bash
npm run dev
# or
pnpm dev
```

This will start the development server at `http://localhost:5173`.

### Client API Mock

There is a simple Client API mocking library that can be extended for offline testing with the development server. 

- `\src\lib\client.mock.ts` 


### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run check` - Run type checking
- `npm run format` - Format code with Prettier
- `npm run lint` - Lint code with ESLint and Prettier

## Building for Production

To create a production build:

```bash
npm run build
# or
pnpm build
```

The build artifacts will be stored in the `dist/` directory.

It will generate a single bundled html file `dist/index.html`

To preview the production build locally:

```bash
npm run preview
# or
pnpm preview
```

## IDE Setup

For the best development experience, we recommend using [VS Code](https://code.visualstudio.com/) with the following extensions:

- [Svelte for VS Code](https://marketplace.visualstudio.com/items?itemName=svelte.svelte-vscode)
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
