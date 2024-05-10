# JWT-Basics
A Node.js authentication system using JSON Web Tokens (JWT). This system includes a login endpoint to generate a JWT upon successful authentication and a protected dashboard endpoint that requires a valid JWT for access.

## Features
- User authentication using JWT
- Token generation upon successful login
- Secure access to the dashboard using a valid JWT

## Getting Started
### Prerequisites
- Node.js installed
- npm or yarn installed
- MongoDB for user data storage

## Usage
### Login
Send a POST request to the `/login` endpoint with the `username` and `password` in the request body.

Example using cURL:
```bash
curl -X POST http://localhost:3000/login -d '{"username": "your-username", "password": "your-password"}' -H "Content-Type: application/json"
```

### Dashboard
To access the dashboard, send a GET request to the `/dashboard` endpoint with the generated JWT in the Authorization header.

Example using cURL:

```bash
curl http://localhost:3000/dashboard -H "Authorization: Bearer your-generated-token"
```
handling, and password protection mechanisms.



