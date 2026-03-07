# 🔐 JWT Auth Service (FastAPI)

A **Python-based authentication backend service** implementing secure user authentication using **JWT tokens**, password hashing, and protected API routes.  
Built using **FastAPI and SQLAlchemy**, this project demonstrates how modern backend systems implement authentication and access control.

---

## 🚀 Features

- User signup with securely hashed passwords
- JWT token generation for authentication
- Protected API routes using OAuth2 Bearer tokens
- SQLite database integration using SQLAlchemy ORM
- Password hashing using bcrypt
- Clean modular backend architecture
- Interactive API documentation using Swagger UI

---

## 🛠 Tech Stack

- Python
- FastAPI
- SQLAlchemy
- SQLite
- Passlib (bcrypt)
- Python-JOSE (JWT)
- Uvicorn

---

## 🏗 Architecture

```text
Client Request
      ↓
FastAPI Authentication API
      ↓
User Authentication Logic
      ↓
Password Hashing (bcrypt)
      ↓
JWT Token Generation
      ↓
SQLite Database (SQLAlchemy)
```

---

## 📂 Project Structure

```
jwt-auth-service/
│
├── main.py          # FastAPI app and API routes
├── models.py        # Database models
├── database.py      # Database connection setup
├── auth.py          # JWT token and password utilities
├── users.db         # SQLite database
└── requirements.txt
```

---

## ⚙ Installation

Clone the repository

```
git clone https://github.com/thearnavmishra/JWT-Auth-Service-FastAPI-.git
cd JWT-Auth-Service-FastAPI-
```

Install dependencies

```
pip install -r requirements.txt
```

---

## ▶ Run the Server

```
uvicorn main:app --reload
```

Server runs at

```
http://127.0.0.1:8000
```

Swagger documentation

```
http://127.0.0.1:8000/docs
```

---

## 🔑 API Endpoints

### User Signup

```
POST /signup
```

Creates a new user account.

---

### User Login

```
POST /login
```

Returns a JWT access token.

---

### Protected Route

```
GET /protected
```

Requires a valid **Bearer Token**.

---

## 🔒 Security Features

- Secure password hashing using bcrypt
- JWT token-based authentication
- OAuth2 password flow implementation
- Protected routes using dependency injection

---

## 📈 Future Improvements

- Refresh token support
- Email verification system
- Password reset workflow
- PostgreSQL database integration
- Docker containerization
- Rate limiting middleware

---

## 👨‍💻 Author

**Arnav Mishra**

GitHub  
https://github.com/thearnavmishra

LinkedIn  
https://www.linkedin.com/in/iamarnavmishra
