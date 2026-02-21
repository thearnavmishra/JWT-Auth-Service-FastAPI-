# 🔐 JWT Auth Service (FastAPI)

Production-ready authentication backend implementing JWT-based login, secure password hashing, and protected API routes using FastAPI and SQLAlchemy.

---

## 🚀 Features

- User signup with hashed passwords
- Secure login with JWT token generation
- Protected routes using OAuth2 Bearer
- SQLite database with SQLAlchemy ORM
- Password hashing using bcrypt
- Clean modular backend structure
- Swagger UI auto documentation

---

## 🛠 Tech Stack

- FastAPI
- Python
- SQLAlchemy
- SQLite
- Passlib (bcrypt)
- Python-JOSE (JWT)
- Uvicorn

---

## 📂 Project Structure

```
jwt-auth-service/
│
├── main.py          # FastAPI app and routes
├── models.py        # Database models
├── database.py      # DB connection
├── auth.py          # JWT + password utils
├── users.db         # SQLite database
└── requirements.txt
```

---

## ⚙️ Installation

```bash
git clone https://github.com/thearnavmishra/JWT-Auth-Service-FastAPI-.git
cd JWT-Auth-Service-FastAPI-
pip install -r requirements.txt
```

---

## ▶️ Run the Server

```bash
uvicorn main:app --reload
```

Server runs at:

```
http://127.0.0.1:8000
```

Swagger docs:

```
http://127.0.0.1:8000/docs
```

---

## 🔑 API Endpoints

### Signup

```
POST /signup
```

Creates a new user.

---

### Login

```
POST /login
```

Returns JWT access token.

---

### Protected Route

```
GET /protected
```

Requires Bearer token.

---

## 🔒 Security Features

- Password hashing with bcrypt
- JWT token authentication
- OAuth2 password flow
- Protected route dependency injection

---

## 📈 Future Improvements

- Refresh tokens
- Email verification
- Password reset flow
- PostgreSQL support
- Docker support
- Rate limiting

---

## 👨‍💻 Author

**Arnav Mishra**

- GitHub: https://github.com/thearnavmishra
- LinkedIn: https://www.linkedin.com/in/iamarnavmishra
