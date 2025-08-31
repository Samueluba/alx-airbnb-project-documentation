# Backend Requirement Specifications

This document outlines the detailed requirements for three core backend features of the Airbnb Clone project: **User Authentication**, **Property Management**, and **Booking System**.  

---

## 1. User Authentication

### Overview
This module handles user registration, login, authentication, and session management using secure methods.

### API Endpoints
- **POST /api/v1/auth/register**
  - Registers a new user.
- **POST /api/v1/auth/login**
  - Authenticates a user and issues a JWT token.
- **GET /api/v1/auth/profile**
  - Retrieves user profile (requires authentication).
- **PUT /api/v1/auth/profile**
  - Updates user profile details.

### Input Specifications
- **Register**
  ```json
  {
    "first_name": "John",
    "last_name": "Doe",
    "email": "john@example.com",
    "password": "StrongPass123!",
    "role": "guest"
  }
