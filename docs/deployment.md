# Deployment

## Deployment Architecture

```txt
Vercel Frontend
  -> Render Backend API
  -> Neon PostgreSQL
```

## Frontend

Platform:

```txt
Vercel
```

Framework:

```txt
Vite / React
```

Environment variable:

```txt
VITE_API_URL
```

Build command:

```bash
npm run build
```

Output directory:

```txt
dist
```

Production URL:

```txt
https://bug-tracker-fullstack-app.vercel.app
```

## Backend

Platform:

```txt
Render
```

Runtime:

```txt
Node.js
```

Environment variables:

```txt
DATABASE_URL
JWT_SECRET
CLIENT_URL
PORT
```

Build command:

```bash
npm install && npx prisma generate && npx prisma migrate deploy
```

Start command:

```bash
npm start
```

## Database

Platform:

```txt
Neon PostgreSQL
```

The database is managed through Prisma ORM.

Main database models:

- User
- Bug

## Production Environment Flow

```txt
User opens Vercel frontend
  -> Frontend sends API request to Render backend
  -> Backend validates JWT token
  -> Backend queries Neon PostgreSQL through Prisma
  -> Backend returns JSON response
  -> Frontend updates UI
```

## Deployment Notes

- Source code is private
- This public repository only documents the project as a case study
- Environment variables are not exposed
- Database credentials are not included
- JWT secrets are not included
- Screenshots and public demo links are safe to show

## Useful Links

Live demo:

```txt
https://bug-tracker-fullstack-app.vercel.app
```

Source code:

```txt
Private repository
```
