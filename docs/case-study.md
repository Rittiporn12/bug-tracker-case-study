# Case Study: Bug Tracker Fullstack App

## Problem

Software teams need a simple way to report, prioritize, and track bugs during development.

Without a clear workflow, bug reports can become scattered, duplicated, or difficult to follow.

## Goal

Build a full-stack bug tracking application that supports authentication, protected routes, bug creation, filtering, status updates, priority updates, and responsive UI.

## My Role

Full-stack developer responsible for:

- Frontend UI
- Backend API
- Authentication
- Database schema
- API integration
- Deployment setup
- Documentation
- Manual testing

## Solution

The application is split into three main parts:

- React frontend for the user interface
- Express backend for REST API endpoints
- PostgreSQL database managed through Prisma ORM

Users can register, log in, create bug reports, view bugs, filter bugs, update status and priority, and delete bugs when allowed.

## Key Decisions

### JWT Authentication

JWT was used to protect private API routes and frontend pages.

### Prisma and PostgreSQL

Prisma was used to model users, bugs, relationships, enums, and database access.

### Responsive UI

The layout was designed to work across desktop, tablet, and mobile devices.

### Light/Dark Mode

A theme toggle was added to improve user experience and demonstrate UI state management.

### Separate Deployment

The frontend and backend were deployed separately:

- Frontend on Vercel
- Backend on Render
- Database on Neon PostgreSQL

## Challenges

### Prisma 7 Adapter Setup

Prisma 7 requires a database adapter. The backend was configured with `@prisma/adapter-pg`.

### Environment Variables

The frontend and backend required separate environment variables for local and production environments.

### Protected API Requests

Axios was configured to attach the JWT token to protected API requests.

### Responsive Navigation

The navbar was adjusted for mobile screens with a collapsible menu.

## Result

The final application supports a complete bug tracking workflow with authentication, protected routes, CRUD functionality, filtering, responsive UI, and deployment-ready configuration.
