# Employee Management System

![Project Demo](https://user-images.githubusercontent.com/74038190/212747903-e9bdf048-2dc8-41f9-b973-0e72ff07bfba.gif)

## Описание

Этот проект — система управления сотрудниками на базе **Spring Boot** с использованием **Spring Data JPA** и **H2 Database** (или любой другой базы данных, поддерживаемой JPA).
Позволяет создавать, получать, обновлять и удалять информацию о сотрудниках через REST API.

## Функционал
- **Добавление сотрудника** (`POST /api/v1/createEmployee`)
- **Получение списка всех сотрудников** (`GET /api/v1/checkEmployee`)
- **Удаление сотрудника по email** (`DELETE /api/v1/deleteEmployee/{email}`)
- **Обновление данных сотрудника (email и зарплата)** (`PUT /api/v1/changeEmployee/{email}`)

## Структура проекта

### 1. Конфигурация
- `EmployeeConfig.java` — содержит предзаполненные данные (закомментировано).

### 2. Контроллеры
- `EmployeeController.java` — REST API для управления сотрудниками.

### 3. Сущность (Entity)
- `Employee.java` — класс-сущность для хранения данных сотрудников в базе данных.

### 4. Репозиторий
- `EmployeeRepository.java` — интерфейс для работы с базой данных через Spring Data JPA.

### 5. Сервис
- `EmployeeService.java` — бизнес-логика приложения, работа с данными сотрудников.

## Установка и запуск

### 1. Клонирование репозитория:
```sh
git clone <URL-репозитория>
cd <папка-репозитория>
```

### 2. Сборка и запуск проекта:
```sh
./mvnw spring-boot:run  # Для Maven
./gradlew bootRun       # Для Gradle
```

### 3. Проверка API
После запуска сервера API доступно по адресу: `http://localhost:8080/api/v1/`

Примеры запросов можно тестировать через **Postman** или **cURL**.

## Требования
- **Java 17+**
- **Spring Boot 3+**
- **Maven/Gradle**

## Контакты
Если у вас есть вопросы, предложения или ошибки, создайте [Issue](https://github.com/your-repo/issues) или свяжитесь со мной.

---
_Этот проект создан в образовательных целях._

