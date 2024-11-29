# RBAC Assignment

## Project Overview
This project implements an authentication and authorization system with Role-Based Access Control (RBAC) using Node.js, Express, and MongoDB.

## Features
- User Registration and Login with JWT-based authentication.
- Middleware for protected routes based on roles.
- Supports roles: Admin, Moderator, User.

## Setup Instructions
1. Clone the repository.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Add a `.env` file with the following content:
   ```env
   JWT_SECRET=your_secret_key
   DB_URL=mongodb://localhost:27017/rbac_assignment
   ```
4. Start the server:
   ```bash
   npm start
   ```

## API Endpoints
- POST `/register` - Register a new user.
- POST `/login` - Login a user and get a JWT token.
- GET `/admin` - Accessible only to Admins.
- GET `/moderator` - Accessible to Admins and Moderators.

