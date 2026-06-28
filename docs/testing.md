# Testing

## Manual Testing Areas

## Authentication

- Register user
- Login user
- Logout user
- Protected route redirect
- Current user lookup

## Bug Management

- Create bug
- View bug list
- Filter bugs by status
- Filter bugs by priority
- View bug detail
- Update bug status
- Update bug priority
- Delete bug

## UI Testing

- Desktop layout
- Tablet layout
- Mobile layout
- Mobile navbar
- Light mode
- Dark mode
- Theme toggle persistence

## API Testing

API endpoints tested with Postman:

```txt
GET /
POST /api/auth/register
POST /api/auth/login
GET /api/auth/me
GET /api/bugs
GET /api/bugs/:id
POST /api/bugs
PATCH /api/bugs/:id
DELETE /api/bugs/:id
```

## Regression Checklist

- Register still works
- Login still works
- Logout still works
- Protected routes still redirect
- Auth token is attached to protected API requests
- Bug list still loads
- Bug filters still work
- Create bug still works
- Bug detail still loads
- Status update still works
- Priority update still works
- Delete bug still works
- Theme toggle still works
- Mobile layout has no horizontal overflow

## Test Notes

Testing was performed manually using:

- Browser testing
- Postman API testing
- Responsive viewport checks
- Production deployment checks
