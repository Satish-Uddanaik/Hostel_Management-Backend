# 🏨 StayEase - Hostel Management System (Backend)

StayEase is a role-based Hostel Management System built using **Spring Boot**. It provides secure REST APIs for managing hostels, students, wardens, room allocation, hostel applications, food confirmation, and payments.

The project is designed to simplify hostel administration by replacing manual processes with a secure and scalable backend application.

---

## ✨ Features

- Student Registration & Login
- JWT Authentication & Authorization
- Role-Based Access (Student & Warden)
- Hostel Management
- Room Allocation
- Hostel Application Management
- Food Confirmation
- Payment Tracking
- RESTful APIs
- MySQL Database Integration

---

## 🛠️ Tech Stack

| Technology | Description |
|------------|-------------|
| Java | Programming Language |
| Spring Boot | Backend Framework |
| Spring MVC | REST API Development |
| Spring Data JPA | Database Operations |
| Spring Security | Authentication & Authorization |
| JWT | Secure Authentication |
| MySQL | Relational Database |
| Lombok | Boilerplate Code Reduction |
| Maven | Dependency Management |
| IntelliJ IDEA | Development IDE |

---

## 📁 Project Structure

```
src
 ├── controller
 ├── service
 ├── repository
 ├── entity
 ├── dto
 ├── security
 ├── config
 ├── exception
 └── resources
```

---

## 🚀 Getting Started

### Prerequisites

- Java 21+
- Maven
- MySQL
- IntelliJ IDEA

### Clone Repository

```bash
git clone https://github.com/your-username/StayEase.git
```

### Configure Database

Update the `application.properties` file.

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/stayease
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### Run the Application

Using Maven

```bash
mvn spring-boot:run
```

Or run the main class directly from IntelliJ IDEA.

---

## 📌 REST API Endpoints

### Authentication

```
POST /auth/register
POST /auth/login
```

### Hostel

```
GET    /hostel/getHostelDetails/{id}
POST   /hostel/create
PUT    /hostel/update/{id}
DELETE /hostel/delete/{id}
```

### Room

```
POST /room/addStudent
GET  /room/{id}
```

### Student

```
GET  /student/{id}
PUT  /student/update
```

> More endpoints are available in the controller package.



