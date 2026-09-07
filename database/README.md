# Database

MySQL database for the Digital Certificate Verification System.

## Technology

* MySQL
* SQL

## Responsibilities

The database layer is responsible for:

* Database design
* Entity and relationship modeling
* Table creation
* Primary keys
* Foreign keys
* Constraints
* Indexes
* Data integrity
* Sample/test data
* Database documentation

## Directory Structure

```text
database/
│
├── schema/
│   ├── 01_create_database.sql
│   ├── 02_create_tables.sql
│   ├── 03_relationships.sql
│   └── 04_indexes.sql
│
├── seed/
│   └── sample_data.sql
│
├── migrations/
│
├── er-diagram/
│   └── er-diagram.png
│
└── README.md
```

## Database Setup

Make sure MySQL Server is installed and running.

Check MySQL:

```bash
mysql --version
```

## SQL Execution Order

Run the SQL files in the following order:

### 1. Create Database

```text
schema/01_create_database.sql
```

### 2. Create Tables

```text
schema/02_create_tables.sql
```

### 3. Create Relationships

```text
schema/03_relationships.sql
```

### 4. Create Indexes

```text
schema/04_indexes.sql
```

### 5. Insert Sample Data

```text
seed/sample_data.sql
```

## Database Design

The database will store information related to:

* Users
* Certificates
* Certificate types
* Verification requests
* Verification results
* Audit information

The final entities and relationships will be based on the approved project requirements.

## Naming Conventions

### Tables

Use lowercase `snake_case`:

```text
users
certificates
verification_requests
```

### Columns

Use lowercase `snake_case`:

```text
user_id
certificate_number
issued_date
created_at
```

### Primary Keys

Use:

```text
<table_name>_id
```

Example:

```text
user_id
certificate_id
```

### Foreign Keys

Use the referenced table's primary key:

```text
user_id
certificate_id
```

## Database Rules

* Every table should have a primary key.
* Foreign keys should be used for relationships.
* Avoid unnecessary duplicate data.
* Use appropriate data types.
* Use constraints to maintain data integrity.
* Add indexes where they improve query performance.
* Never commit database passwords or credentials.
* Schema changes should be documented.

## ER Diagram

The ER diagram is maintained in:

```text
er-diagram/
```

## Development

Create a database feature branch:

```bash
git checkout -b feature/database-<feature-name>
```

After making changes:

```bash
git add database/
git commit -m "feat: update database schema"
git push origin feature/database-<feature-name>
```

Create a Pull Request before merging into `main`.

## Database Change Policy

Any change to the database structure should be reflected in the appropriate SQL file or migration.

Examples:

```text
Adding a table       → schema
Adding an index      → schema
Changing structure   → migrations
Adding test data     → seed
Updating ER diagram  → er-diagram
```
