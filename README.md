## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Project setup

```bash
$ npm install
```

## Database Setup with Prisma

This project uses Prisma as the ORM for database management.

### Initializing the Database Schema

1. Ensure your database is running and the `DATABASE_URL` environment variable is set in a `.env` file.

2. To initialize the schema without migrations (for development):

```bash
$ npm run prisma:push
```

This pushes the schema directly to the database.

### Creating and Running Migrations

1. To create a new migration after modifying `prisma/schema.prisma`:

```bash
$ npm run prisma:migrate
```

This creates a migration file and applies it to the database.

2. To generate the Prisma client:

```bash
$ npm run prisma:generate
```

Run this after any schema changes to update the generated client code.

### Using Prisma Studio

To open Prisma Studio for database visualization and editing:

```bash
$ npm run prisma:studio
```

Prisma Studio will open in your browser at `http://localhost:5555`.

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

With Mau, you can deploy your application in just a few clicks, allowing you to focus on building features rather than managing infrastructure.
