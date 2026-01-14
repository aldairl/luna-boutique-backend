## Description

🧩 Overview

Built with NestJS, leveraging a modular and domain-oriented architecture with dependency injection to ensure scalability, maintainability, and testability.

Data persistence is handled using PostgreSQL and Prisma ORM, with a well-defined relational schema and versioned migrations. The application is ready to run on modern Node.js environments and can be deployed on free-tier hosting services.

🛠️ Tech Stack
Backend: NestJS (TypeScript)
Architecture: Modular, domain-driven, dependency injection
Database: PostgreSQL
ORM: Prisma
Language: TypeScript
Runtime: Node.js

## Project setup

```bash
$ npm install
```

## Database Setup with Prisma

1. Ensure your database is running and the `DATABASE_URL` environment variable is set in a `.env` file.
In production create a .env.production file.

2. Generate the Prisma client:

```bash
$ npm run prisma:generate
```

Run this after any schema changes to update the generated client code.

## Compile and run the project

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Run tests

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Deployment
[deployment documentation](https://docs.nestjs.com/deployment) for more information.

```bash
$ npm install -g @nestjs/mau
$ mau deploy
```

## prisma scrips

To initialize the schema without migrations (for development):

```bash
$ npm run prisma:push
```

This pushes the schema directly to the database.

### Creating and Running Migrations

To create a new migration after modifying `prisma/schema.prisma`:

```bash
$ npm run prisma:migrate
```

This creates a migration file and applies it to the database.


To open Prisma Studio for database visualization and editing:

```bash
$ npm run prisma:studio
```

Prisma Studio will open in your browser at `http://localhost:5555`.