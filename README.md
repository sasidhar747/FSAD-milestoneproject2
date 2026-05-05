# Smart Campus Event Management System

Professional Spring Boot web application for managing campus events, workshops, seminars, and student registrations.

## Features
- Student sign up and login.
- Browse upcoming events through MVC pages.
- Filter events by department, type, and date.
- Register for events with server-side validation.
- View personal registrations and submit feedback.
- Admin CRUD operations for events.
- Registration statistics with aggregate insights.
- REST APIs for event listings and event statistics.
- Global exception handling with Spring MVC.
- HTTP Basic authentication for admin pages.

## Technology Stack
- Java 17+
- Spring Boot 3.2
- Spring MVC
- Spring Data JPA
- Spring Security
- Thymeleaf
- H2 Database
- Maven Wrapper

## Demo Accounts
- Student:
  - Email: `student@univ.edu`
  - Password: `student123`
- Admin:
  - Email: `admin@univ.edu`
  - Password: `admin123`

## Run the Project
1. Open a terminal in the project folder.
2. Start the application:

```powershell
.\mvnw.cmd spring-boot:run
```

3. Open `http://localhost:8081`.

## REST API
- `GET /api/events`
- `GET /api/events/{id}`
- `GET /api/events?department=Computer Science&type=Workshop&date=2026-05-10`
- `GET /api/events/stats`

## Admin Access
- Admin dashboard: `http://localhost:8081/admin/dashboard`
- Admin routes use the browser's HTTP Basic authentication prompt.

## H2 Console
- URL: `http://localhost:8081/h2-console`
- JDBC URL: `jdbc:h2:mem:campusdb`
- Username: `sa`
- Password: `password`
