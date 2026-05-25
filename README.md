# 🔐 Python Fullstack Task 2
## User Authentication System
A Python Fullstack Web Application built using Flask, SQLite and Werkzeug Security.

---

## 📋 Project Overview

This is a secure **User Authentication System** that extends Task 1 by adding user registration, login, session management, and access control. The application demonstrates backend security fundamentals using Flask sessions and password hashing.

---

## ✅ Features Implemented

1. ✅ User Registration (Signup) with hashed password storage
2. ✅ User Login with session-based authentication
3. ✅ Protected Dashboard (accessible only after login)
4. ✅ Secure Logout (clears session)
5. ✅ Password Hashing using Werkzeug Security
6. ✅ Clean UI with styled forms and pages

---

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| Python | Backend logic |
| Flask | Web framework |
| SQLite | Database storage |
| Werkzeug | Password hashing & security |
| Flask Session | Session-based authentication |
| HTML | Frontend structure |
| CSS | Styling and design |

---

## 📁 Project Structure

```
python_fullstack_task2/
│
├── app.py                 → Flask backend (auth routes & database logic)
├── database.db            → SQLite database (stores user credentials)
├── static/
│   └── style.css          → CSS styling for UI
└── templates/
    ├── register.html      → Registration form
    ├── login.html         → Login form
    └── dashboard.html     → Protected dashboard page
```

---

## ▶️ How to Run

**Step 1 - Clone the repository:**
```bash
git clone https://github.com/kavyatn089/python_fullstack_task2
```

**Step 2 - Go into the project folder:**
```bash
cd python_fullstack_task2
```

**Step 3 - Install required packages:**
```bash
pip install flask werkzeug
```

**Step 4 - Run the application:**
```bash
python app.py
```

**Step 5 - Open in browser:**
```
http://127.0.0.1:5000/register
```

---

## 🗄️ Database Design

### Table: `users`

| Column | Type | Description |
|--------|------|-------------|
| id | INTEGER (Primary Key) | Auto-incremented user ID |
| username | TEXT (UNIQUE) | Unique username |
| password | TEXT (Hashed) | Bcrypt hashed password |

---

## 🔄 How It Works

```
User fills Registration form
          ↓
Password is hashed using Werkzeug
          ↓
Username + Hashed Password saved in SQLite
          ↓
User fills Login form
          ↓
Flask checks credentials from database
          ↓
Session is created on successful login
          ↓
User is redirected to Protected Dashboard
          ↓
Logout clears the session
```

---

## 🔐 Authentication Flow

```
/register  →  POST  →  Hash password  →  Save to DB  →  Redirect to /login
/login     →  POST  →  Verify hash    →  Set session →  Redirect to /dashboard
/dashboard →  GET   →  Check session  →  Show page   →  (or redirect to /login)
/logout    →  GET   →  Clear session  →  Redirect to /login
```

---

## 📸 Output Screenshots

### 📝 Registration Page
> User enters a unique username and password to create an account.
> Password is hashed before storing — never saved as plain text.

![Register Page](screenshots/register.png)

---

### 🔑 Login Page
> User enters credentials. Flask verifies the hashed password using Werkzeug.

![Login Page](screenshots/login.png)

---

### 🏠 Dashboard Page
> Protected page accessible only to logged-in users.
> Displays a welcome message with the username from session.

![Dashboard Page](screenshots/dashboard.png)

---

## 🛡️ Security Concepts Applied

| Concept | Implementation |
|--------|---------------|
| Password Hashing | `generate_password_hash()` from Werkzeug |
| Password Verification | `check_password_hash()` from Werkzeug |
| Session Management | Flask built-in `session` object |
| Protected Routes | Check `'user' in session` before rendering |
| Secure Logout | `session.pop('user', None)` to clear session |

---

## 🎯 Learning Outcomes

- ✅ Implemented secure user registration with password hashing
- ✅ Built login system with session-based authentication
- ✅ Protected routes from unauthorized access
- ✅ Applied Werkzeug security for password management
- ✅ Managed user sessions correctly using Flask
- ✅ Understood real-world authentication workflows

---

## 📚 References

- [Flask Sessions Documentation](https://flask.palletsprojects.com/en/latest/quickstart/#sessions)
- [Werkzeug Security](https://werkzeug.palletsprojects.com)
- [OWASP Password Guidelines](https://owasp.org/www-project-top-ten/)

---

## 👩‍💻 Author

**Kavya**
- GitHub: [@kavyatn089](https://github.com/kavyatn089)

---

## 📅 Date

May 2026 🔐 Python Fullstack Task 2
## User Authentication System
A Python Fullstack Web Application built using Flask, SQLite and Werkzeug Security.



## 📋 Project Overview

This is a secure **User Authentication System** that extends Task 1 by adding user registration, login, session management, and access control. The application demonstrates backend security fundamentals using Flask sessions and password hashing.



## ✅ Features Implemented

1. ✅ User Registration (Signup) with hashed password storage
2. ✅ User Login with session-based authentication
3. ✅ Protected Dashboard (accessible only after login)
4. ✅ Secure Logout (clears session)
5. ✅ Password Hashing using Werkzeug Security
6. ✅ Clean UI with styled forms and pages



## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| Python | Backend logic |
| Flask | Web framework |
| SQLite | Database storage |
| Werkzeug | Password hashing & security |
| Flask Session | Session-based authentication |
| HTML | Frontend structure |
| CSS | Styling and design |



## 📁 Project Structure


python_fullstack_task2/
│
├── app.py                 → Flask backend (auth routes & database logic)
├── database.db            → SQLite database (stores user credentials)
├── static/
│   └── style.css          → CSS styling for UI
└── templates/
    ├── register.html      → Registration form
    ├── login.html         → Login form
    └── dashboard.html     → Protected dashboard page




## ▶️ How to Run

**Step 1 - Clone the repository:**
```bash
git clone https://github.com/kavyatn089/python_fullstack_task2
```

**Step 2 - Go into the project folder:**
```bash
cd python_fullstack_task2
```

**Step 3 - Install required packages:**
```bash
pip install flask werkzeug
```

**Step 4 - Run the application:**
```bash
python app.py
```

**Step 5 - Open in browser:**
```
http://127.0.0.1:5000/register
```

---

## 🗄️ Database Design

### Table: `users`

| Column | Type | Description |
|--------|------|-------------|
| id | INTEGER (Primary Key) | Auto-incremented user ID |
| username | TEXT (UNIQUE) | Unique username |
| password | TEXT (Hashed) | Bcrypt hashed password |

---

## 🔄 How It Works

```
User fills Registration form
          ↓
Password is hashed using Werkzeug
          ↓
Username + Hashed Password saved in SQLite
          ↓
User fills Login form
          ↓
Flask checks credentials from database
          ↓
Session is created on successful login
          ↓
User is redirected to Protected Dashboard
          ↓
Logout clears the session
```

---

## 🔐 Authentication Flow

```
/register  →  POST  →  Hash password  →  Save to DB  →  Redirect to /login
/login     →  POST  →  Verify hash    →  Set session →  Redirect to /dashboard
/dashboard →  GET   →  Check session  →  Show page   →  (or redirect to /login)
/logout    →  GET   →  Clear session  →  Redirect to /login
```

---

## 📸 Output Screenshots

### 📝 Registration Page
> User enters a unique username and password to create an account.
> Password is hashed before storing — never saved as plain text.

![Register Page](screenshots/register.png)

---

### 🔑 Login Page
> User enters credentials. Flask verifies the hashed password using Werkzeug.

![Login Page](screenshots/login.png)

---

### 🏠 Dashboard Page
> Protected page accessible only to logged-in users.
> Displays a welcome message with the username from session.

![Dashboard Page](screenshots/dashboard.png)

---

## 🛡️ Security Concepts Applied

| Concept | Implementation |
|--------|---------------|
| Password Hashing | `generate_password_hash()` from Werkzeug |
| Password Verification | `check_password_hash()` from Werkzeug |
| Session Management | Flask built-in `session` object |
| Protected Routes | Check `'user' in session` before rendering |
| Secure Logout | `session.pop('user', None)` to clear session |

---

## 🎯 Learning Outcomes

- ✅ Implemented secure user registration with password hashing
- ✅ Built login system with session-based authentication
- ✅ Protected routes from unauthorized access
- ✅ Applied Werkzeug security for password management
- ✅ Managed user sessions correctly using Flask
- ✅ Understood real-world authentication workflows

---

## 📚 References

- [Flask Sessions Documentation](https://flask.palletsprojects.com/en/latest/quickstart/#sessions)
- [Werkzeug Security](https://werkzeug.palletsprojects.com)
- [OWASP Password Guidelines](https://owasp.org/www-project-top-ten/)

---

## 👩‍💻 Author

**Kavya**
- GitHub: [@kavyatn089](https://github.com/kavyatn089)

---

## 📅 Date

May 2026
