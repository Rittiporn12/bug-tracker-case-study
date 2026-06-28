# Architecture

## System Overview

```txt
User
  -> React Frontend
  -> Axios API Client
  -> Express Backend
  -> Prisma ORM
  -> PostgreSQL Database
```

## Frontend

The frontend is built with React and Vite.

Responsibilities:

- Page routing
- Login and registration forms
- Authentication state
- Protected routes
- API requests
- Responsive UI
- Light/dark theme toggle

## Backend

The backend is built with Node.js and Express.

Responsibilities:

- Authentication endpoints
- Bug management endpoints
- JWT validation middleware
- Request validation
- Database operations
- Error responses

## Database

The database uses PostgreSQL.

Main models:

- User
- Bug

Main relationships:

- A user can report many bugs
- A user can be assigned many bugs
- A bug must have one reporter
- A bug can optionally have one assignee

## Deployment

```txt
Vercel Frontend
  -> Render Backend API
  -> Neon PostgreSQL
```

## Request Flow

```txt
1. User interacts with the React frontend
2. Axios sends API requests to the Express backend
3. Express validates requests and checks JWT authentication
4. Prisma handles database queries
5. PostgreSQL stores user and bug data
6. API returns JSON response to the frontend
```
