# My-SQL-Projects
This repository contains SQL projects showcasing my skills in writing queries, joins, aggregations, and data analysis. Created as part of my learning journey into data and technology.
<br><br>
## 📁 Project 1:
<br><br>
## Student Results Database Design

This project illustrates a simple relational database schema for managing student results.  
It includes three tables — **Student**, **Class**, and **Results** — connected through primary and foreign keys.

### Skills Demonstrated
- Database design and ER modelling  
- Understanding PK/FK relationships  
- Logical data structuring  
- Diagram creation using Draw.io  

### Tables
- Student(id, name)
- Class(class_id, class_name)
- Results(result_id, student_id, class_id, mark)

![Student Results Database Diagram](student_results_database.drawio.png)
<br><br>

## 📁 Project 2:
<br><br>

## 🗄️ SQL Data Analysis Projects

A collection of SQL projects completed as part of my **Data Technician Bootcamp**, showcasing database design and query-writing skills applied to retail and sales data scenarios.

## 🧰 Skills Demonstrated

### Core Querying
- **SELECT / SELECT DISTINCT** – retrieving specific columns and unique values from tables
- **WHERE** – filtering records based on single and multiple conditions (e.g. category, date range, boolean flags)
- **ORDER BY** – sorting results in ascending/descending order to surface top and bottom values
- **GROUP BY** – aggregating data by category (e.g. summarising records per country, product, or customer group)
- **HAVING** – filtering aggregated results (e.g. groups with counts or totals above a threshold)
- **BETWEEN / LIKE** – range-based and pattern-based filtering of records

### Aggregation & Functions
- **COUNT, SUM, MAX, AVG** – calculating totals, counts, and averages across grouped data
- Combining aggregate functions with `GROUP BY` and `ORDER BY` to rank and compare results

### JOINs & Relational Design
- Understanding and applying different types of **table JOINs** to combine related data across multiple tables
- Designing a relational **database schema** for a retail business, including:
  - **Inventory**, **Sales**, **Customer**, and **Loyalty** tables
  - Defining **Primary Keys (PK)** and **Foreign Keys (FK)** to establish relationships between tables
- Writing SQL statements to **CREATE** tables and **INSERT** initial data

### Subqueries
- Using nested subqueries to filter results against calculated values (e.g. records above the overall average, or the maximum value within a group)

## 📁 Project Context
- Designed a relational database structure for a small retail business (inventory, sales, customer, and loyalty data)
- Practised writing and debugging SQL queries against a real dataset using **PostgreSQL (via Supabase)**
- Used queries to extract insights such as top categories, records within a range, and grouped summaries — the same querying logic used to analyse retail and sales data

## 🎯 Purpose
These projects were built to strengthen core SQL skills relevant to a **Data Technician** role — from designing efficient relational databases to writing queries that extract clear, actionable insights from structured data.

---

<br><br>


## 📁 Project 3:
<br><br>
## Employee & Training Records Database (SQL)

A relational database project built to track employees and the training courses they've completed. Created as part of my **Data Technician Bootcamp**.

### 📖 Overview

This project models a simple but realistic business scenario: a company needs to keep track of its employees and which training courses each of them has completed (e.g. for compliance or skills tracking purposes). It demonstrates core relational database design and SQL querying skills.

## 🗂️ Database Schema

Two related tables, linked by `EmployeeID`:

**Employees**

| Column        | Type          | Constraint   |
|---------------|---------------|--------------|
| EmployeeID    | VARCHAR(10)   | PRIMARY KEY  |
| EmployeeName  | VARCHAR(100)  | NOT NULL     |
| JobRole       | VARCHAR(100)  |              |

**TrainingRecords**

| Column            | Type          | Constraint                        |
|-------------------|---------------|------------------------------------|
| TrainingRecordID  | VARCHAR(10)   | PRIMARY KEY                        |
| EmployeeID        | VARCHAR(10)   | NOT NULL, FOREIGN KEY → Employees  |
| Course            | VARCHAR(100)  | NOT NULL                           |


## 🧰 Skills Demonstrated
- Designing normalised relational tables with **PRIMARY KEY** and **FOREIGN KEY** constraints
- Enforcing data integrity with **NOT NULL**
- Populating tables using **INSERT INTO ... VALUES**
- Querying and filtering data with **SELECT** and **WHERE**
- Using **subqueries** to pull related data from another table

## 🎯 Purpose

This project was built to strengthen my understanding of relational database design and SQL fundamentals as part of my transition into a career in data and technology.

<br><br>
## 📁 Project 4:
<br><br>
# Student Scoring & Customer Shipping Database (SQL)

A SQL project is covering database querying across multiple related datasets — student performance records, customer shipping/order data — to practise extracting insights from structured data.

## 📖 Overview

This project brings together several tables (**Studentscoring**, **Shippings**, **Customers**, **Orders**) to practise core SQL querying techniques: filtering, sorting, grouping, aggregating, and joining data across tables to answer real business-style questions.

## 🧰 Skills Demonstrated

### Core Querying
- **SELECT / SELECT DISTINCT** – retrieving specific columns and unique values (e.g. distinct customers with pending deliveries)
- **WHERE** – filtering records on single and combined conditions (e.g. score thresholds, age ranges, country, delivery status)
- **ORDER BY** – sorting results ascending/descending (e.g. top-scoring students, most recent shipments)
- **LIMIT** – restricting result sets to a defined number of rows (e.g. top 3 scores)
- **LIKE** – pattern-matching text values (e.g. customers whose first name starts with "J")
- **BETWEEN** – filtering values within a range (e.g. age range for a targeted score update)

### Aggregation & Grouping
- **GROUP BY** – summarising data by category (e.g. average score by country, total customers by country)
- **HAVING** – filtering grouped/aggregated results (e.g. countries with more than one student)
- **COUNT / AVG** – calculating totals and averages across grouped records

### Table JOINs
- Using **JOIN** to combine related tables (e.g. matching shipping records to customer names via a shared customer ID)

### Data Modification
- **UPDATE** – amending existing records based on conditions (e.g. updating scores, delivery status, or customer country)
- **INSERT INTO ... SELECT** – inserting new records derived from existing query results
- **DELETE** – removing records based on a condition

## 📁 Datasets Used
- **Studentscoring** – student names, scores, country, and age
- **Shippings** – shipping status and linked customer
- **Customers** – customer details including name, age, and country
- **Orders** – customer order history

## 🎯 Purpose
These queries were built to strengthen core SQL skills relevant to a **Data Technician** role — filtering, sorting, grouping, joining, and updating structured data to extract clear, actionable insights, in the same way retail and sales data would be analysed in a real business setting.

---
*Part of my ongoing journey transitioning into a career in data and technology.*
