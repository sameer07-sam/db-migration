# MySQL to PostgreSQL Migration Project

## Overview

This project demonstrates how to migrate data from a MySQL database to a PostgreSQL database using Python.

## Files

- `mysql_schema.sql`: MySQL schema and sample data for the `users` table.
- `postgres_schema.sql`: PostgreSQL schema for the `users` table.
- `migrate_mysql_to_postgres.py`: Python script for migrating the data.
- `requirements.txt`: Python dependencies.
- `SUMMARY_REPORT.md`: Summary of migration process and results.

## Instructions

### 1. Prepare Databases

- Set up MySQL and PostgreSQL servers.
- Run `mysql_schema.sql` in MySQL and `postgres_schema.sql` in PostgreSQL to create the `users` table.

### 2. Configure Credentials

- Edit `migrate_mysql_to_postgres.py` and update the `mysql_config` and `postgres_config` dictionaries with your actual database credentials.

### 3. Install Python Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run Migration Script

```bash
python migrate_mysql_to_postgres.py
```
- The script fetches all users from MySQL and inserts them into PostgreSQL.

### 5. Verify Data Integrity

- Check both databases to ensure the data matches.

## Data Integrity

- All columns and primary keys are preserved.
- For complex schemas, additional mapping and scripts may be required.

---

For more details, see `SUMMARY_REPORT.md`.