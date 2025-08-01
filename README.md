# Bash Database Management System (DBMS)

A simple command-line Database Management System written entirely in **Bash** as part of the ITI DevOps Training Program (2025).  
Made by **Ahmed Maher**

---

## Overview

This project is a lightweight DBMS that mimics basic SQL-like database operations using Bash scripting. It supports interactive CLI-based database and table manipulation with validation.

---

## Project Structure

All databases are stored under a folder named `DBMS/`.  
Each database is a directory, and each table consists of two files:

- `table_name.txt`: Contains actual row data
- `table_name_schema.txt`: Contains column names and data types

Example:
```
DBMS/
└── my_database/
    ├── users.txt
    └── users_schema.txt
```

---

## Features

### Database Operations

- Create a new database
- List existing databases
- Connect to a specific database
- Drop a database

### Table Operations (within a connected database)

- Create a table with column definitions and data types
- List all tables
- Drop a table
- Insert records with validation (including primary key check)
- Select records (full, specific columns, filtered)
- Update specific fields in records
- Delete records based on conditions

---

## Data Types & Rules

- Supported data types: `int`, `string`
- The **first column** in every table is the **Primary Key**
  - Must be unique and not empty
- Table and column naming rules:
  - Must start with a letter
  - May only contain letters, numbers, or underscores

---

## Input Validation

- All user input is validated
  - Primary key must be unique
  - Data types must match declared types
  - Names must follow required naming rules


---

## Usage Instructions

### 1. Make the script executable

```bash
chmod +x dbms.sh
```

### 2. Run the application

```bash
./dbms.sh
```

---

## Main Menu Options

```
1. Create Database
2. List Databases
3. Connect To Database
4. Drop Database
5. Exit
```

---

## Table Menu Options (Inside a Database)

```
1. Create Table
2. List Tables
3. Drop Table
4. Insert into Table
5. Select From Table
6. Delete From Table
7. Update Table
8. Back to Main Menu
```


---

## Author

**Ahmed Maher**  
ITI DevOps Track – 2025

---
