# 💊 MedTracker

A full-stack **Online Medication and Prescription System** built using:

* ⚙️ Spring Boot (Backend)
* 🎨 React (Frontend)
* 🗄️ MySQL (Database)

This application allows users to manage medications, track schedules, and maintain health-related data efficiently.

---

## 🚀 Features

* 🔐 User Authentication (Register & Login)
* 💊 Medication Management
* ⏰ Schedule Tracking
* 📡 RESTful API Integration
* 🌐 Full-stack architecture

---

## 🛠️ Prerequisites

Make sure you have the following installed:

* Java 17+
* Node.js & npm
* MySQL Server (running on localhost:3306)
* Maven (or use Maven Wrapper)

---

## ⚙️ Backend Setup

📁 Folder: `medication-tracker-backend`

### 1. Create Database

Run this in MySQL:

```sql
CREATE DATABASE medication_db;
```

---

### 2. Configure Database Credentials

Open:

```
src/main/resources/application.properties
```

Update:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/medication_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

---

### 3. Run Backend Server

```bash
./mvnw spring-boot:run
```

Backend will start at:
👉 http://localhost:8080

---

## 🎨 Frontend Setup

📁 Folder: `medication-tracker-frontend`

### 1. Install Dependencies

```bash
npm install
```

---

### 2. Run Frontend

```bash
npm start
```

Frontend will start at:
👉 http://localhost:3000

---

## 🔗 API Endpoints

| Feature  | Method | Endpoint       |
| -------- | ------ | -------------- |
| Register | POST   | /auth/register |
| Login    | POST   | /auth/login    |

📌 Base URL:

```
http://localhost:8080
```

---

## 🧪 API Testing

You can test APIs using:

* Postman
* cURL
* PowerShell Script:

```
C:\Users\lavan\.gemini\antigravity\brain\e9c6fe04-7e15-49af-935e-305137286627\test_api.ps1
```

---

## 📂 Project Structure

```
medication-tracker/
│
├── medication-tracker-backend/
│   ├── src/
│   └── pom.xml
│
├── medication-tracker-frontend/
│   ├── src/
│   └── package.json
│
└── README.md
```

---

## ⚠️ Common Issues & Fixes

### Port Already in Use

```properties
server.port=8081
```

---

### MySQL Connection Failed

* Ensure MySQL is running
* Verify username and password
* Check database name

---

### CORS Issues

* Enable CORS in backend configuration

---

## 🌟 Future Enhancements

* 📱 Mobile App Integration
* 🔔 Notification & Reminder System
* 📊 Health Analytics Dashboard
* ☁️ Cloud Deployment (AWS / Firebase)

---
