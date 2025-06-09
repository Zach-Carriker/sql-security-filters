# sql-security-filters

# 🧮 SQL Security Filters: Investigating Login Activity & Employee Workstations

This project demonstrates the use of SQL queries with filters to investigate suspicious login activity and perform system update planning based on employee department and location data. The queries are structured around two database tables: `log_in_attempts` and `employees`.

---

## 🧠 Project Scenario

As part of an effort to improve the organization's security posture, I was tasked with:
- Investigating suspicious or failed login attempts
- Identifying employee machines needing workstation updates based on department and office location
- Reporting the findings to company stakeholders

The queries shown in this project were written using `WHERE` clauses and SQL logical operators to filter and analyze activity from organizational data.

---

## 📊 Key Queries and Goals

### 🔐 Investigate Login Activity

- **Retrieve failed login attempts after 6:00 PM**
- **Retrieve login attempts on or around a specific date**
- **Retrieve login attempts from outside of Mexico**

### 🧑‍💼 Employee Workstation Updates

- **Find all employees in the Marketing department located in East offices**
- **Find all employees in Finance or Sales departments**
- **Find all employees not in the Information Technology department**

Each query includes explanation of the logic and filter operators used (e.g., `AND`, `OR`, `NOT`, `LIKE`, `%`, `=`, `>`) to demonstrate control over SQL conditionals.

---

## 🗃 Database Schema

### `log_in_attempts` Table
| Column        | Description                                |
|---------------|--------------------------------------------|
| event_id      | Login event ID                             |
| username      | Employee's username                        |
| login_date    | Date of login attempt                      |
| login_time    | Time of login attempt                      |
| country       | Country of login                           |
| ip_address    | IP address of login source                 |
| success       | Indicates if login was successful (TRUE/FALSE) |

### `employees` Table
| Column        | Description                                |
|---------------|--------------------------------------------|
| employee_id   | Unique ID assigned to the employee         |
| device_id     | ID of the employee’s device                |
| username      | Username assigned to the employee          |
| department    | Department the employee works in           |
| office        | Physical office location of the employee   |

---

## 📎 Supporting Documents

- [📄 Apply_Filters_in_SQL_Queries.pdf](Apply_Filters_in_SQL_Queries.pdf) – Includes the SQL queries, explanations, and scenario context.
- [📄 SQL_Table_Format.pdf](SQL_Table_Format.pdf) – Schema documentation for the `log_in_attempts` and `employees` tables.

---

> 🗒️ *This project is based on a fictional scenario and is intended for educational purposes.*
