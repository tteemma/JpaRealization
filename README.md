# Employee Management System

![Worker](https://user-images.githubusercontent.com/74038190/212748830-4c709398-a386-4761-84d7-9e10b98fbe6e.gif)

## Description

This project is an **Employee Management System** built with **Spring Boot**, using **Spring Data JPA** and **H2 Database** (or any other JPA-supported database). 
It allows creating, retrieving, updating, and deleting employee information via REST API.

## Features
- **Add an employee** (`POST /api/v1/createEmployee`)
- **Retrieve all employees** (`GET /api/v1/checkEmployee`)
- **Delete an employee by email** (`DELETE /api/v1/deleteEmployee/{email}`)
- **Update employee details (email and salary)** (`PUT /api/v1/changeEmployee/{email}`)

## Project Structure

### 1. Configuration
- `EmployeeConfig.java` — contains preloaded employee data (commented out).

### 2. Controllers
- `EmployeeController.java` — REST API controller for managing employees.

### 3. Entity
- `Employee.java` — entity class for storing employee details in the database.

### 4. Repository
- `EmployeeRepository.java` — interface for database operations using Spring Data JPA.

### 5. Service
- `EmployeeService.java` — business logic handling employee data.

## Installation & Run

### 1. Clone the repository:
```sh
git clone <repository-URL>
cd <repository-folder>
```

### 2. Build and start the project:
```sh
./mvnw spring-boot:run  # For Maven
./gradlew bootRun       # For Gradle
```

### 3. API Testing
Once the server is running, the API is available at: `http://localhost:8080/api/v1/`

You can test the API using **Postman** or **cURL**.

## Requirements
- **Java 17+**
- **Spring Boot 3+**
- **Maven/Gradle**

## Contact
<a href="https://github.com/https://github.com/tteemma" target="_blank">
<img src=https://img.shields.io/badge/github-%2324292e.svg?&style=for-the-badge&logo=github&logoColor=white alt=github style="margin-bottom: 5px;" />
</a>
<a href="https://gitlab.com/https://gitlab.se.ifmo.ru/Temo4ka" target="_blank">
<img src=https://img.shields.io/badge/gitlab-330F63.svg?&style=for-the-badge&logo=gitlab&logoColor=white alt=gitlab style="margin-bottom: 5px;" />
</a>
<a href="https://t.me/ttemmaaa" target="_blank">
  <img src="https://img.shields.io/badge/telegram-0088cc.svg?&style=for-the-badge&logo=telegram&logoColor=white" alt="telegram" style="margin-bottom: 5px;" />
</a>

---
_This project was created for educational purposes._

