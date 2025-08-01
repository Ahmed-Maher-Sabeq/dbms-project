# Bash Database Management System (DBMS)

A simple command-line Database Management System written entirely in **Bash** as part of the ITI DevOps Training Program (2025). 


---

## Features

- Create, list, connect to, and drop databases
- Create, list, and drop tables with schema definition
- Primary key enforcement on the first column
- Insert, select, update, and delete records
- Supports basic filtering and column selection
- Data types supported: `int`, `string`
- Fully interactive CLI menus
- Data stored as flat `.txt` files

---

## Directory Structure

All databases and their contents are stored under the `./DBMS` directory.

Each database is a folder, and each table has:
- A `.txt` file for data
- A `_schema.txt` file for column names and data types

DBMS/
└── my_database/
├── my_table.txt
└── my_table_schema.txt


---

## How to Run

1. Give the script execute permission:
   ```bash
   chmod +x dbms.sh

    Run the script:

    ./dbms.sh

Main Menu Options

1. Create Database         → Initializes a new database (directory)
2. List Databases          → Lists all created databases
3. Connect To Database     → Opens table-level menu for a specific DB
4. Drop Database           → Deletes a database and its contents
5. Exit                    → Exits the application

Table Menu Options (After Connecting to a Database)

1. Create Table            → Define table schema (columns and types)
2. List Tables             → Lists tables in current DB
3. Drop Table              → Deletes a table and its schema
4. Insert into Table       → Adds a new row (with PK validation)
5. Select From Table       → Full, partial, or filtered select
6. Delete From Table       → Deletes rows based on column match
7. Update Table            → Updates row values where a condition is met
8. Back to Main Menu       → Return to main DB menu

Supported Data Types

    int: Integer values (10, -5, etc.)

    string: Any text (including special characters)

Note: The first column is always treated as the Primary Key. It must be unique and not empty.
Input & Validation Rules

    Database and table names must:

        Start with a letter

        Contain only letters, numbers, and underscores

    Column names follow the same rules

    Input is validated for:

        Data type correctness

        Primary key uniqueness

        Schema constraints

Author

Ahmed Maher
Part of the ITI DevOps Track – 2025
