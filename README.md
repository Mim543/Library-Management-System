# 📚 Library Management System

<div align="center">

![Library Management System](https://img.shields.io/badge/Project-Library%20Management%20System-blue)

![React](https://img.shields.io/badge/Frontend-React.js-61DAFB?logo=react)
![Node](https://img.shields.io/badge/Backend-Node.js-339933?logo=node.js)
![Express](https://img.shields.io/badge/Framework-Express.js-000000?logo=express)
![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?logo=mysql)
![JWT](https://img.shields.io/badge/Auth-JWT-orange)
![GitHub](https://img.shields.io/badge/Version-Control-black?logo=github)

### 🚀 Full Stack Library Management System

A modern web-based application designed to automate and manage library operations efficiently.

</div>

---

# 📖 Project Overview

The Library Management System is a full-stack web application that helps libraries manage books, members, borrowing records, returns, fines, and reports.

This project is developed as part of the Database Systems, Database Lab, and Software Engineering courses.

---

# 🎯 Objectives

* Manage library books efficiently
* Maintain member records
* Track book borrowing and returns
* Calculate overdue fines automatically
* Generate reports and analytics
* Provide a secure authentication system

---

# 🏗️ System Architecture

```text
Frontend (React.js)
        │
        ▼
REST API (Node.js + Express.js)
        │
        ▼
MySQL Database
```

---

# 🛠️ Technology Stack

## Frontend

* React.js
* Tailwind CSS
* React Router DOM
* Axios

## Backend

* Node.js
* Express.js
* JWT Authentication
* bcrypt.js

## Database

* MySQL
* MongoD

## Development Tools

* Git
* GitHub
* VS Code
* Postman
* MySQL Workbench

---

# ✨ Features

## 🔐 Authentication

* User Registration
* User Login
* JWT Authentication
* Password Encryption
* Role-Based Authorization

---

## 📚 Book Management

* Add Books
* Edit Books
* Delete Books
* Search Books
* View Book Details
* Book Availability Tracking

---

## 👨‍🎓 Member Management

* Register Members
* Update Member Information
* Delete Members
* View Member Profiles

---

## 📖 Borrowing Management

* Issue Books
* Return Books
* Renew Books
* Borrowing History

---

## 💰 Fine Management

* Automatic Fine Calculation
* Overdue Tracking
* Fine Reports

---

## 📊 Reports & Analytics

* Daily Reports
* Monthly Reports
* Borrow Statistics
* Fine Collection Reports
* Dashboard Analytics

---

# 👥 User Roles

## Administrator

* Manage Users
* Manage Librarians
* Generate Reports
* View Analytics

## Librarian

* Manage Books
* Manage Members
* Issue Books
* Return Books
* Generate Reports

## Student / Member

* Search Books
* View Borrowed Books
* View Fine Information
* Update Profile

---

# 🗂️ Project Structure

```bash
library-management-system/
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── layouts/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── routes/
│   │   ├── hooks/
│   │   ├── context/
│   │   └── App.jsx
│   │
│   └── package.json
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── validations/
│   ├── utils/
│   ├── server.js
│   └── package.json
│
├── database/
│   ├── schema.sql
│   ├── seed.sql
│   └── triggers.sql
│
├── docs/
│   ├── SRS.pdf
│   ├── ERD.png
│   ├── DFD.png
│   ├── UseCases.pdf
│   └── Reports.pdf
│
├── README.md
└── .gitignore
```

---

# 🗄️ Database Modules

### Users

```sql
user_id
name
email
password
role
created_at
```

### Books

```sql
book_id
title
author
isbn
category
quantity
available_quantity
```

### Members

```sql
member_id
name
email
phone
address
```

### Borrows

```sql
borrow_id
member_id
book_id
issue_date
due_date
return_date
status
```

### Fines

```sql
fine_id
borrow_id
amount
status
```

---

# 🚀 Installation Guide

## Clone Repository

```bash
git clone https://github.com/your-username/library-management-system.git
```

```bash
cd library-management-system
```

---

## Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

Frontend runs on:

```bash
http://localhost:5173
```

---

## Backend Setup

```bash
cd backend

npm install

npm run dev
```

Backend runs on:

```bash
http://localhost:5000
```

---

## Database Setup

Create database:

```sql
CREATE DATABASE library_management_system;
```

Import schema:

```sql
SOURCE schema.sql;
```

Import seed data:

```sql
SOURCE seed.sql;
```

---

# 🔑 Environment Variables

Create `.env`

```env
PORT=5000

DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=library_management_system

JWT_SECRET=your_secret_key
```

---

# 📋 API Endpoints

## Authentication

```http
POST /api/auth/register
POST /api/auth/login
```

## Books

```http
GET    /api/books
GET    /api/books/:id
POST   /api/books
PUT    /api/books/:id
DELETE /api/books/:id
```

## Members

```http
GET    /api/members
POST   /api/members
PUT    /api/members/:id
DELETE /api/members/:id
```

## Borrowing

```http
POST /api/borrow
POST /api/return
GET  /api/history
```

---

# 🔒 Security Features

* JWT Authentication
* Password Hashing (bcrypt)
* Input Validation
* SQL Injection Prevention
* Role-Based Access Control
* Protected Routes

---

# 🧪 Testing

### Backend Testing

```bash
npm test
```

### API Testing

Use:

* Postman
* Thunder Client

---

# 📅 Development Roadmap

### Phase 1

* Requirements Analysis
* SRS Documentation
* DFD
* Use Cases

### Phase 2

* ER Diagram
* Database Design
* Normalization

### Phase 3

* Backend Development
* REST API

### Phase 4

* Frontend Development

### Phase 5

* Testing
* Deployment
* Documentation

---

# 📈 Future Enhancements

* QR Code Integration
* Barcode Scanner
* Email Notifications
* Mobile App
* Online Reservation
* AI Book Recommendation System

---

# 🤝 Contributors

### Mim Akter

Department of Artificial Intelligence and Data Science

Green University of Bangladesh

---

# 📜 License

This project is developed for educational and academic purposes.

---

<div align="center">

### ⭐ If you like this project, don't forget to star the repository!

Made with ❤️ using React, Node.js, Express.js and MySQL

</div>
