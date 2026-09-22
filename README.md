# 🎓 Smart Outpass Management System

A full-stack web application developed to automate and streamline the hostel outpass approval process in educational institutions.

The system provides role-based access for **Students, Wardens, Security Staff, and Administrators**, enabling digital outpass requests, approval workflows, real-time status tracking, and secure campus exit management.

The project is built using **Spring Boot**, **React.js**, **PostgreSQL**, **JWT Authentication**, and **REST APIs**.

---

# 🌟 Key Features

## 👨‍🎓 Student Module

- Apply for outpass requests online
- View outpass history
- Edit pending requests
- Track approval status
- View profile information

## 👮 Warden Module

- Review student requests
- Approve or reject outpasses
- Add comments and remarks
- Monitor student requests

## 🛡️ Security Module

- Verify approved outpasses
- Check-in and check-out management
- Track active passes
- Monitor daily student movement

## 👨‍💼 Admin Module

- User management
- Student management
- Warden management
- Security staff management
- Password reset functionality
- System monitoring

## 🔐 Authentication & Security

- JWT Authentication
- Role-Based Access Control (RBAC)
- Secure REST APIs
- Protected Routes
- Spring Security Integration

---

# 🧰 Tech Stack

## Backend

- Java 17+
- Spring Boot
- Spring Security
- Spring Data JPA
- Hibernate
- Maven

## Frontend

- React.js
- JavaScript
- HTML5
- CSS3
- React Router

## Database

- PostgreSQL

## Authentication

- JWT (JSON Web Tokens)

## Tools

- Git
- GitHub
- VS Code
- IntelliJ IDEA
- Postman

---

# ⚡ System Modules

## Student

- Apply Outpass
- Edit Outpass
- View Outpass
- Outpass History
- Student Dashboard

## Warden

- Review Outpass
- Approve / Reject Requests
- Warden Dashboard

## Security

- Active Passes
- Check-In / Check-Out
- Security Dashboard

## Admin

- User Registration
- User Management
- Password Reset
- Admin Dashboard

---

# 📦 Installation & Setup

## 1️⃣ Clone Repository

```bash
git clone https://github.com/AllanSibi/smart-outpass-management-system.git

cd smart-outpass-management-system
```

---

## 2️⃣ Backend Setup

Navigate to backend folder:

```bash
cd outpass-backendv1-main
```

### Configure Database

Update:

```properties
src/main/resources/application.properties
```

Example:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/outpass_management

spring.datasource.username=postgres

spring.datasource.password=postgres
```

---

### Run Backend

Using Maven:

```bash
mvn spring-boot:run
```

or

```bash
./mvnw spring-boot:run
```

Backend runs on:

```text
http://localhost:8080
```

---

## 3️⃣ Frontend Setup

Navigate to frontend folder:

```bash
cd outpass-frontendv3-main
```

Install dependencies:

```bash
npm install
```

Run React application:

```bash
npm start
```

Frontend runs on:

```text
http://localhost:3000
```

---

# 📁 Project Structure

```text
smart-outpass-management-system/
│
├── outpass-backendv1-main/
│   ├── src/main/java/com/mit/outpass
│   │   ├── controller
│   │   ├── service
│   │   ├── repository
│   │   ├── entity
│   │   ├── dto
│   │   ├── config
│   │   ├── exception
│   │   └── enums
│   │
│   ├── src/main/resources
│   └── pom.xml
│
├── outpass-frontendv3-main/
│   ├── src
│   │   ├── components
│   │   │   ├── admin
│   │   │   ├── auth
│   │   │   ├── common
│   │   │   ├── security
│   │   │   ├── student
│   │   │   └── warden
│   │   │
│   │   ├── services
│   │   ├── context
│   │   └── utils
│   │
│   └── package.json
│
└── README.md
```

---

# 🚀 Application Workflow

1. Student logs into the system
2. Student submits an outpass request
3. Warden reviews the request
4. Warden approves/rejects request
5. Security verifies approved pass
6. Student checks out
7. Security records return entry
8. System maintains complete history

---

# 🔐 Authentication Flow

```text
User Login
      │
      ▼
Spring Security
      │
      ▼
JWT Token Generated
      │
      ▼
Frontend Stores Token
      │
      ▼
Protected API Access
```

---

# 📊 Features by Role

| Role | Features |
|--------|----------|
| Student | Apply, Edit, Track Outpass |
| Warden | Approve, Reject, Review Requests |
| Security | Verify Passes, Check-In/Out |
| Admin | Manage Users and System |

---

# 📡 REST API Modules

## Authentication APIs

```text
/api/auth/*
```

## Student APIs

```text
/api/student/*
```

## Warden APIs

```text
/api/warden/*
```

## Security APIs

```text
/api/security/*
```

## Admin APIs

```text
/api/admin/*
```

---

# 🧪 Common Issues

## ❌ PostgreSQL Connection Failed

Verify:

```properties
spring.datasource.url

spring.datasource.username

spring.datasource.password
```

---

## ❌ Port 8080 Already In Use

Change:

```properties
server.port=8081
```

or stop existing process.

---

## ❌ npm install Errors

Clear cache:

```bash
npm cache clean --force
```

Then:

```bash
npm install
```

---

## ❌ CORS Errors

Verify:

```java
CorsConfiguration
```

and

```java
SecurityConfig.java
```

configuration.

---

# 🔮 Future Enhancements

- Mobile Application
- Email Notifications
- SMS Alerts
- QR Code Based Verification
- Face Recognition Integration
- Analytics Dashboard
- Multi-Hostel Support
- Cloud Deployment
- Audit Logs
- Parent Notification System

---

# 🎯 Learning Outcomes

This project demonstrates:

- Spring Boot Development
- React Frontend Development
- REST API Design
- JWT Authentication
- Role-Based Access Control
- PostgreSQL Integration
- Full Stack Application Development

---

# 🤝 Contributing

Fork the repository

Create a new branch

```bash
git checkout -b feature/new-feature
```

Commit changes

```bash
git commit -m "Add new feature"
```

Push changes

```bash
git push origin feature/new-feature
```

Create a Pull Request.

---

# 👨‍💻 Author

**Allan Sibi A S**

🎓 Information Technology Student  
🏫 Madras Institute of Technology (MIT), Chennai  
💻 Aspiring Software Engineer

GitHub:
https://github.com/AllanSibi

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

---

✨ Smart Outpass Management System – A Full Stack Hostel Outpass Automation Platform built using Spring Boot, React, PostgreSQL, JWT Authentication, and REST APIs.
