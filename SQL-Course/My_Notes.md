# 📘 SQL Study Notes
**My daily notes, definitions, and code examples.**

Database: PostgreSQL  
Tool: pgAdmin

## 📑 Table of Contents (Index)
1. [Section 1: Setup & Installation](#section-1-setup--installation)
2. [Section 2: Fundamentals (SELECT, WHERE, DISTINCT, ORDER BY, LIMIT, BETWEEN, IN, LIKE, ILIKE)](#section-2-fundamentals)
3. [Section 3: Group By & Aggregations](#section-3-group-by--aggregations)
4. [Section 4: JOINS (Inner, Left, Right, Outer)](#section-4-joins-inner-left-right-outer)
5. [Section 5: Advanced Commands (Timestamps, Math)](#section-5-advanced-commands-timestamps-math)
6. [Section 6: Assessment Test 2](#section-6-assessment-test-2)
7. [Section 7: Creating Databases](#section-7-creating-databases)
8. [Section 8: Creating Tables & Data Types](#section-8-creating-tables--data-types)
9. [Section 9: Conditional Expressions (CASE, COALESCE)](#section-9-conditional-expressions-case-coalesce)
10. [Section 10: Advanced SQL (Window Functions & CTEs)](#section-10-advanced-sql-window-functions--ctes)
11. [Section 11: Python & SQL Integration](#section-11-python--sql-integration)

---

## Section 1: Setup & Installation
* **Goal:** Get PostgreSQL running.
* Installed PostgreSQL 16.
* Configured pgAdmin 4.
* Restored the `dvdrental` database.

[↑ Back to Top](#sql-study-notes)

---
Database would be having tables
 ## TABLE in SQL is like a grid
It has:

Rows → go left to right

Columns → go top to bottom

Columns = headings (what kind of information)

Columns tell us WHAT type of data we are storing.


Rows = one full entry (one person / one thing)

Each row is one complete record.

Very important line (remember this)

Column = WHAT

Row = WHO / WHICH ONE

Table Student

How SQL sees it
Column = vertical (⬇️)
Name
Age
Class

Row = horizontal (➡️)
Rohan | 10 | 5

## Section 2: Fundamentals (SELECT, WHERE, ORDER BY , LIMIT,BETWEEN , IN ,LIKE, ILIKE)
### SELECT Statement
Retrieves data from a table.
```sql
SELECT coloumn_name
FROM table_name;

--Can select multiple coloums
select coloumn_1, coloumn_2
from table_1

-- For selecting all the coloumn

Select *
From table


