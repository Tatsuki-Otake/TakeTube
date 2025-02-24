# TakeTube
This is a youtube clone built with Next.js, Clerk, Drizzle, and Neon.

# Description
## 01 Setup
- Configure environment
  - runtime (Node.js, Bun)
  - package manager (bun)
- Why bun?
  - You will get the same environment as I do
  - Easily run TypeScript scripts with ES6 imports
  - Less issues with dependency issues regarding React19
    - (npm throws an error, yarn throws a warning, bun simply works)
- Establish basic Bun commands
  - bun add === npm install
  - bunx === npx
- Create next.js project
  - use exact version
  - add shadcn/ui
  - get familiar with the structure
- Add useful VSCode(Cursor) extensions

## 02 Basic layout
- Add logo asset
- Learn basic app router folders
- Sidebar component
  - Sidebar sections
  - Sidebar items
- Navbar
  - Search input
  - Sign in compornent

## 03 Authentication
- Integrate Clerk
- Add Sign in screens
- Add UserButton
- Add middleware
- Use auth state on sidebar sections
- Protect routes

## 04 Database setup
- Create a PostgreSQL database (www.neon.tech)
- Setup DrizzleORM
- Create users schema
- Migrate changes to database
- Learn how to use drizzle-kit
- Why DrizzleORM?
  - Only ORM with both relational and SQL-like query APIs
  - Serverless by default
  - Forcing us to "understand" our queries

## 05 Webhook sync
- Create ngrok account (or any other local tunnel solution)
- Obtain a static domain (not required, but easier development)
- Add script to concurrently run local tunnel & app
- Create the users webhook
- Connect the webhook on Clerk dashboard

## 06 tRPC setup
- Why tRPC?
  - end-to-end typesafety
  - familiar hooks (useQuery, useMutation etc.)
  - v11 allows us to do authenticated prefetching
