## Description

clean arquitecture

## Project setup

```bash
$ npm install
```

## Database Setup with Prisma

1. Ensure your database is running and the `DATABASE_URL` environment variable is set in a `.env` file.

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