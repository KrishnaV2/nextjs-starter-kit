# Next.js Starter Kit

Powered by Better-T-Stack.

## Features

- **TypeScript** - For type safety and improved developer experience
- **Next.js** - Full-stack React framework
- **TailwindCSS** - Utility-first CSS for rapid UI development
- **shadcn/ui** - Reusable UI components
- **Drizzle** - TypeScript-first ORM
- **PostgreSQL** - Database engine
- **Authentication** - Better-Auth
- **Oxc** - Linter + Formatter
- **Husky + Lint-Staged** - Pre-commit hooks

## Getting Started

First, install the dependencies:

```bash
pn install
```

## Database Setup

This project uses PostgreSQL with Drizzle ORM.

1. Make sure you have a PostgreSQL database set up.
2. Update your `.env` file with your PostgreSQL connection details.

3. Apply the schema to your database:

```bash
pn run db:push
```

Then, run the development server:

```bash
pn run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the fullstack application.

## Project Structure

```
nextjs-starter-kit/
├── app/
│   └── api/         # Next.js API
├── components/
│   └── ui/          # ShadcnUI Components
├── lib/
│   ├── auth/        # Authentication configuration & logic (Better-Auth)
│   ├── db/          # Database schema & queries (drizzle-orm)
│   └── env/         # Typed and Verified env vars
```

## Available Scripts

- `pn run dev`: Start all applications in development mode
- `pn run build`: Build all applications
- `pn run check-types`: Check TypeScript types across all apps
- `pn run db:push`: Push schema changes to database
- `pn run db:studio`: Open database studio UI
