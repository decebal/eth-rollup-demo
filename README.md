## What's included

[Next.js](https://nextjs.org/) - Framework<br>
[Turborepo](https://turbo.build) - Build system<br>
[Biome](https://biomejs.dev) - Linter, formatter<br>
[TailwindCSS](https://tailwindcss.com/) - Styling<br>
[Shadcn](https://ui.shadcn.com/) - UI components<br>
[TypeScript](https://www.typescriptlang.org/) - Type safety<br>
[i18n](https://next-international.vercel.app/) - Internationalization<br>
[Sentry](https://sentry.io/) - Error handling/monitoring<br>

## Directory Structure

```
my-monorepo/
├── apps/
│   ├── admin/                # Admin interface (React/Vercel)
│   ├── rollup/               # Rollup deployment and scripts
│   ├── proxyd/               # Proxyd service with dynamic auth
├── infra/
│   ├── pulumi/               # Pulumi IaC scripts
│   └── environments/         # Environment-specific configs
│       ├── dev/
│       ├── staging/
│       └── prod/
├── packages/
│   ├── core/                 # Core utilities (Go libraries)
│   ├── db/                   # Database utilities and migrations
│   ├── contracts/            # Optimism contracts and deployment logic
│   ├── shared/               # Shared types, constants, and schemas
│   └── ui/                   # Shared UI components (Shadcn)
├── scripts/                  # Automation scripts
├── .turbo/                   # Turborepo cache
├── turbo.json                # Turborepo config
├── package.json              # Root package configuration
├── tsconfig.base.json        # Shared TypeScript config
└── README.md                 # Documentation
```

## Prerequisites

Bun<br>
Docker<br>
Sentry<br>

## Getting Started

Clone this repo locally with the following command:

```bash
//TODO
```

1. Install dependencies using bun:

```sh
bun i
```

2. Copy `.env.example` to `.env` and update the variables.

```sh
# Copy .env.example to .env for each app
//TODO
cp apps/web/.env.example apps/web/.env
```

4. Start the development server from either bun or turbo:

```ts
//TODO
bun dev // starts everything in development mode (web, app, api, email)
bun dev:web // starts the web app in development mode
bun dev:app // starts the app in development mode
bun dev:api // starts the api in development mode
bun dev:email // starts the email app in development mode

// Database
bun migrate // run migrations
bun seed // run seed
```
