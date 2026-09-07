# Backend

Java / Spring Boot backend for the Digital Certificate Verification System.

## Technology

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* MySQL
* Maven

## Responsibilities

The backend handles:

* REST APIs
* Business logic
* Authentication and authorization
* Certificate management
* Certificate verification
* Database communication
* Input validation
* Error handling

## Project Structure

```text
backend/
├── src/
│   ├── main/
│   │   ├── java/
│   │   └── resources/
│   │
│   └── test/
│
├── pom.xml
└── README.md
```

## Architecture

The backend follows a layered architecture:

```text
Controller
    ↓
Service
    ↓
Repository
    ↓
MySQL Database
```

### Controller

Handles HTTP requests and responses.

### Service

Contains application and business logic.

### Repository

Handles database operations.

### Model / Entity

Represents database entities.

### DTO

Defines data transferred between the frontend and backend.

## Setup

Make sure Java and Maven are installed.

Check Java:

```bash
java -version
```

Check Maven:

```bash
mvn -version
```

Build the project:

```bash
mvn clean install
```

Run the application:

```bash
mvn spring-boot:run
```

Default development server:

```text
http://localhost:8080
```

## Database

The backend connects to the MySQL database maintained in:

```text
../database/
```

Database credentials should be stored in environment-specific configuration and must not be committed to Git.

## Development

Create a feature branch:

```bash
git checkout -b feature/backend-<feature-name>
```

Commit changes:

```bash
git add backend/
git commit -m "feat: <description>"
```
