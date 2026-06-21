# Task Management Application

A full-stack Task Management Application developed using **Flask**, **SQLite**, **HTML**, **CSS**, and **Bootstrap**. The application allows users to create, manage, update, and track tasks efficiently through a secure authentication system and an intuitive user interface.

## 📌 Project Overview

The Task Management Application is designed to help users organize and monitor their daily tasks. Users can register, log in securely, create tasks, update task details, track progress, and delete completed tasks. The project demonstrates practical implementation of authentication, CRUD operations, database integration, and responsive web design.

This project was developed as part of the **Thiranex Internship Program** to showcase full-stack web development skills and database management concepts.

---

## 🚀 Features

### 🔐 User Authentication

- User Registration
- User Login
- Secure Password Hashing using bcrypt
- Session Management
- Logout Functionality

### 📋 Task Management

- Create New Tasks
- View All Tasks
- Edit Existing Tasks
- Delete Tasks
- Track Task Progress

### 📊 Task Status Tracking

Each task can have one of the following statuses:

- Pending
- In Progress
- Completed

### 🎯 Priority Management

Tasks can be categorized as:

- High Priority
- Medium Priority
- Low Priority

### 📱 Responsive Design

- Mobile Friendly
- Tablet Friendly
- Desktop Friendly

### 🔍 Additional Features

- Search Tasks
- Filter Tasks by Status
- Sort Tasks by Due Date
- Dashboard Statistics

---

## 💻 Technologies Used

### Frontend

- HTML5
- CSS3
- Bootstrap 5
- JavaScript

### Backend

- Python
- Flask

### Database

- SQLite

### Security

- Flask-Bcrypt
- Session Management

### Development Tools

- VS Code
- Git
- GitHub

---

## 📂 Project Structure

```text
task-management-app/
│
├── app.py
├── database.db
├── requirements.txt
│
├── templates/
│   ├── login.html
│   ├── register.html
│   ├── dashboard.html
│   ├── add_task.html
│   ├── edit_task.html
│   └── task_list.html
│
├── static/
│   ├── css/
│   │   └── style.css
│   │
│   ├── js/
│   │   └── script.js
│   │
│   └── images/
│
└── README.md
```

---

## 🗄 Database Schema

### Users Table

```sql
CREATE TABLE users(
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    username TEXT UNIQUE NOT NULL,
    password TEXT NOT NULL
);
```

### Tasks Table

```sql
CREATE TABLE tasks(
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    title TEXT NOT NULL,
    description TEXT,
    due_date DATE,
    priority TEXT,
    status TEXT,
    user_id INTEGER,
    FOREIGN KEY(user_id) REFERENCES users(id)
);
```

---

## ⚙️ Installation Guide

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/task-management-application.git
cd task-management-application
```

### Step 2: Create Virtual Environment

```bash
python -m venv venv
```

### Step 3: Activate Virtual Environment

#### Windows

```bash
venv\Scripts\activate
```

#### Mac/Linux

```bash
source venv/bin/activate
```

### Step 4: Install Dependencies

```bash
pip install flask flask-bcrypt
```

### Step 5: Run the Application

```bash
python app.py
```

### Step 6: Open Browser

```text
http://127.0.0.1:5000
```

---

## 📋 Application Workflow

### User Registration

Users create an account by providing:

- Username
- Password

Passwords are securely hashed before storage.

### User Login

Registered users can log in securely using their credentials.

### Create Task

Users can add tasks with:

- Title
- Description
- Due Date
- Priority Level

### Manage Tasks

Users can:

- View Tasks
- Edit Tasks
- Update Status
- Delete Tasks

### Dashboard

The dashboard displays:

- Total Tasks
- Pending Tasks
- In Progress Tasks
- Completed Tasks

---

## 📸 Screenshots

### Registration Page

- User registration form

### Login Page

- Secure login interface

### Dashboard

- Task overview and statistics

### Add Task Page

- Task creation form

### Task List Page

- View and manage tasks

### Edit Task Page

- Update task information

---

## 🔒 Security Features

### Password Hashing

Passwords are encrypted using bcrypt before being stored in the database.

### Session Management

Authenticated sessions are maintained securely using Flask sessions.

### Input Validation

User input is validated to prevent invalid data entry.

### SQL Injection Prevention

Parameterized database queries are used throughout the application.

---

## 🎯 Learning Outcomes

This project demonstrates:

- Full Stack Web Development
- Flask Framework
- Database Integration
- User Authentication
- CRUD Operations
- Session Handling
- Responsive Design
- Secure Coding Practices
- Version Control with Git and GitHub

---

## 🔮 Future Enhancements

- Email Notifications
- Due Date Reminders
- Task Categories
- Team Collaboration
- Real-Time Updates using WebSockets
- Dark Mode
- Calendar Integration
- File Attachments

---

## 📈 Expected Outcome

A fully functional task management system that enables users to efficiently organize, track, and manage their tasks through a secure and responsive web application.

---

## 👨‍🎓 Internship Information

**Internship Program:** Thiranex Internship Program

**Domain:** Full Stack Web Development

**Project:** Task Management Application

---

## 👤 Author

**Dharani Prathipati**

Computer Science Engineering Student

GitHub: https://github.com/DharaniP-27

LinkedIn: Add Your LinkedIn Profile Link

---

## 📄 License

This project is developed for educational and internship purposes. Free to use and modify for learning and academic projects.# thiranex-task-2
