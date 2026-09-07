# Digital Certificate Verification System

A web-based Digital Certificate Verification System designed to issue, manage, and verify digital certificates securely.

## Tech Stack

* **Frontend:** React
* **Backend:** Java / Spring Boot
* **Database:** MySQL

## Project Structure

```text
digital-certificate-verification-system/
│
├── frontend/          # React frontend
│
├── backend/           # Java / Spring Boot backend
│
├── database/          # MySQL database and SQL scripts
│
├── docs/              # Project documentation
│
├── .gitignore
├── LICENSE
└── README.md
```

## Architecture

```text
React Frontend
       │
       │ REST API
       ▼
Java / Spring Boot
       │
       │ JDBC / JPA
       ▼
     MySQL
```

## Team Responsibilities

### Frontend

Responsible for:

* User interface
* Certificate search and verification screens
* Authentication interfaces
* Dashboard
* API integration

### Backend

Responsible for:

* REST APIs
* Business logic
* Authentication and authorization
* Certificate processing
* Database integration

### Database

Responsible for:

* MySQL database design
* Tables and relationships
* Primary and foreign keys
* Constraints
* Indexes
* Sample data
* Database documentation
* ER diagram

## Database

All database-related files are maintained inside:

```text
database/
```

The database structure is divided into:

```text
database/
├── schema/
├── seed/
├── migrations/
└── er-diagram/
```

## Getting Started

Clone the repository:

```bash
git clone <repository-url>
cd digital-certificate-verification-system
```

Follow the README files inside the respective directories for frontend, backend, and database setup instructions.

## Development

Create a feature branch before working:

```bash
git checkout -b feature/<feature-name>
```

After completing your work:

```bash
git add .
git commit -m "feat: description of change"
git push origin feature/<feature-name>
```

Create a Pull Request to merge the feature into `main`.

## Status

🚧 Project under development.
