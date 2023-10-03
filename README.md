# Full Stack E-Commerce + Dashboard & CMS Project 
## Technologies used: Next.js 13 App Router, React, Tailwind, Prisma, MySQL
### Key Features:
- I'm using Shadcn UI for the Admin interface.
- My admin dashboard is functioning as a CMS, Admin, and API.
- I'm managing multiple vendors and stores through this single CMS, generating API routes for each.
- I'm handling category, product, and filter management, including image uploads and updates.
- I'm managing "Billboards" and their association with categories or standalone display.
- I'm implementing a search feature for all aspects, including pagination.
- I'm controlling featured products on the homepage and overseeing orders and sales, tracking revenue with graphs.
- Clerk is handling Authentication.
- I'm managing order creation and utilizing Stripe checkout and webhooks.
- I'm using MySQL + Prisma + PlanetScale for the database setup.

### Prerequisites
**Node version 14.x**
### Cloning the repository

```shell
git clone https://github.com/abishek-as/ecommerce-dashboard-cms.git
```

### Install packages

```shell
npm i
```

### Setup .env file


```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# This was inserted by `prisma init`:
# Environment variables declared in this file are automatically made available to Prisma.
# See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

# Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB and CockroachDB.
# See the documentation for all the connection string options: https://pris.ly/d/connection-strings

DATABASE_URL=''
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""
STRIPE_API_KEY=
FRONTEND_STORE_URL=http://localhost:3001
STRIPE_WEBHOOK_SECRET=
```

### Connect to PlanetScale and Push Prisma
```shell
npx prisma generate
npx prisma db push
```


### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `dev`           | Starts a development instance of the app |
