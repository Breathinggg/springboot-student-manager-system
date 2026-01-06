# Student Management System

> A university course project from 2022 - A comprehensive student management system built with Spring Boot.

**Note: The UI is in Chinese (Simplified Chinese).**

## Overview

This is a full-featured Student Management System developed as a course project during my undergraduate studies in 2022. The system supports three user roles: **Student**, **Teacher**, and **Administrator**.

## Features

- **Student Management** - CRUD operations for student records
- **Teacher Management** - Manage teacher profiles
- **Class Management** - Organize students into classes
- **Course Management** - Create and manage courses
- **Course Enrollment** - Student course registration
- **Attendance Tracking** - Record student attendance
- **Leave Management** - Leave request and approval workflow
- **Score Management** - Grade recording, import/export, and statistics charts

## Tech Stack

| Component | Technology |
|-----------|------------|
| Backend | Spring Boot 2.0.1 |
| ORM | MyBatis |
| Template Engine | Thymeleaf |
| Frontend UI | EasyUI |
| Database | MySQL 5.5+ |
| Build Tool | Maven |
| JDK | Java 1.8 |

## Screenshots

![Login Page](项目截图/1.png)

![Dashboard](项目截图/2.png)

![Student List](项目截图/3.png)

![Course Management](项目截图/4.png)

![Score Statistics](项目截图/5.png)

![Attendance](项目截图/6.jpg)

## Getting Started

### Prerequisites

- JDK 1.8
- MySQL 5.5+
- Maven 3.x

### Database Setup

1. Create database `studentmanager`
2. Import `sql.sql`
3. Update `src/main/resources/application.yml`:

```yaml
spring:
  datasource:
    url: jdbc:mysql://127.0.0.1:3306/studentmanager
    username: root
    password: your_password
```

### Run

```bash
mvn clean install
mvn spring-boot:run
```

Visit http://localhost:8080

### Default Accounts

| Role | Username | Password |
|------|----------|----------|
| Admin | admin | 123456 |
| Student | 王小明 | 123456 |
| Teacher | 赵老师 | 111 |

## Project Structure

```
src/main/java/com/wdd/studentmanager/
├── controller/     # Controllers
├── service/        # Business logic
├── mapper/         # MyBatis mappers
├── domain/         # Entity classes
├── config/         # Configuration
├── interceptors/   # Login interceptor
└── util/           # Utilities
```

## License

This project is for educational purposes only.

---

*University Course Project - 2022*
