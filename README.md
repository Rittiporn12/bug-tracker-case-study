# Bug Tracker Fullstack App - Case Study

A public case study for a full-stack bug tracking system built with React, Express, PostgreSQL, Prisma, and JWT authentication.

## Live Demo

[Open Live Demo](https://bug-tracker-fullstack-app.vercel.app)

## Preview

![Dashboard](./screenshots/dashboard.png)

## Overview

Bug Tracker Fullstack App is a web application for reporting, tracking, filtering, and updating software bugs. The project includes authentication, protected routes, bug management, responsive UI, and light/dark mode.

This repository is a public showcase only. The source code is private.

## Key Features

- User registration and login
- JWT authentication
- Protected routes
- Create bug reports
- View bug list
- Filter bugs by status and priority
- View bug details
- Update bug status
- Update bug priority
- Delete bug reports with permission checks
- Responsive UI for desktop, tablet, and mobile
- Light and dark mode

## Tech Stack

| Area           | Technology                       |
| -------------- | -------------------------------- |
| Frontend       | React, Vite, React Router, Axios |
| Backend        | Node.js, Express                 |
| Database       | PostgreSQL, Prisma               |
| Authentication | JWT, bcryptjs                    |
| Deployment     | Vercel, Render, Neon PostgreSQL  |

## Screenshots

### Login

![Login](./screenshots/login-light.png)

### Dashboard

![Dashboard](./screenshots/dashboard.png)

### Bug List

![Bug List](./screenshots/bug-list.png)

### Bug Detail

![Bug Detail](./screenshots/bug-detail.png)

### Mobile Responsive

![Mobile](./screenshots/mobile.png)

## Architecture

```txt
User
  -> React Frontend
  -> Express REST API
  -> Prisma ORM
  -> PostgreSQL Database
```

## What I Built

- Designed and implemented the frontend UI
- Built authentication flow with JWT
- Created protected frontend routes
- Created protected backend API routes
- Built the bug CRUD workflow
- Added bug filtering by status and priority
- Integrated Prisma with PostgreSQL
- Added responsive design
- Added light/dark mode
- Deployed frontend and backend separately
- Wrote API, database, deployment, and testing documentation

## Testing

Manual testing covered:

- Register user
- Login user
- Logout user
- Protected route redirect
- Create bug
- View bug list
- Filter bugs
- View bug detail
- Update bug status
- Update bug priority
- Delete bug
- Responsive layout
- Light/dark mode

## Source Code

The source code is private.

This repository is a public case study and project showcase for portfolio review.
