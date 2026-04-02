# 🤝 API Contract: Local Auth Pilot

## Base URL
`http://localhost:8080/api/v1`

## Authentication Flow
1. User sends credentials to `/login`.
2. Server returns a **JWT Access Token**.
3. App includes token in `Authorization: Bearer <token>` header for protected routes.

## Endpoints

### POST /login
**Description:** Authenticate user and return a session token.

**Request Body:**
```json
{
  "email": "string (required)",
  "password": "string (required)"
}
```

**Success Response (200 OK):**
```json
{
  "email": "string (required)",
  "password": "string (required)"
}
```

**Error Response (401 Unauthorized):**
```json
{
  "error": "Invalid email or password"
}
```



