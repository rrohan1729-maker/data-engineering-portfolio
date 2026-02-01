# 📘 SQL Study Notes
**My daily notes, definitions, and code examples**

**Database:** PostgreSQL  
**Tool:** pgAdmin

---

## 📑 Table of Contents (Index)
1. [Section 1: Setup & Installation](#section-1-setup--installation)
2. [Section 2: Fundamentals](#section-2-fundamentals-select-where-distinct-order-by-limit-between-in-like-ilike)
3. [Section 3: Group By & Aggregations](#section-3-group-by--aggregations)
4. [Section 4: JOINS](#section-4-joins-inner-left-right-outer)
5. [Section 5: Advanced Commands](#section-5-advanced-commands-timestamps-math)
6. [Section 6: Assessment Test 2](#section-6-assessment-test-2)
7. [Section 7: Creating Databases](#section-7-creating-databases)
8. [Section 8: Creating Tables & Data Types](#section-8-creating-tables--data-types)
9. [Section 9: Conditional Expressions](#section-9-conditional-expressions-case-coalesce)
10. [Section 10: Advanced SQL](#section-10-advanced-sql-window-functions--ctes)
11. [Section 11: Python & SQL Integration](#section-11-python--sql-integration)

---

## Section 1: Setup & Installation
**Goal:** Get PostgreSQL running.

- Installed PostgreSQL 16
- Configured pgAdmin 4
- Restored the `dvdrental` database

---

## Understanding Tables in SQL

A **table** in SQL is like a **grid**.

### Rows
- Go **left to right**
- Each row = **one complete record**

### Columns
- Go **top to bottom**
- Each column = **type of data**

### Remember
- **Column = WHAT**
- **Row = WHO / WHICH ONE**

### Example: Student Table

| Name  | Age | Class |
|------|-----|-------|
| Rohan | 10  | 5     |

---

## Section 2: Fundamentals (SELECT, WHERE, DISTINCT, ORDER BY, LIMIT, BETWEEN, IN, LIKE, ILIKE)

### SELECT
Used to retrieve data from a table.

```sql
SELECT coloumn
FROM table;
```
---If select all data can use *

```sql
Select *
from table
```

---We can select multiple coloums also

```sql
select coloumn_1, coloumn_2, coloumn_3
from table
```
### Business Problem 1: Customer Marketing List

**Context:**  
The marketing team wants to send a promotional email campaign.

**Requirement:**  
Retrieve the **first name**, **last name**, and **email address** of all customers.

**SQL Solution:**

```sql
SELECT first_name, last_name, email
FROM customer;
```





   
