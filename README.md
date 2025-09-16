# 🗂️ Employee Database Project (MySQL)

## 📌 Overview
This project is a **mini Employee Management Database** built using **MySQL**.  
It demonstrates how to create relational tables, insert sample data, and run queries for learning and practice.  

The project covers:-
- Designing relational database tables  
- Using `INSERT`, `JOIN`, `GROUP BY`, `LIMIT`, `DELETE` and window functions  
- Running **real-world interview-style queries**  

---

## 🎯 Objective :-
- To practice **SQL database creation and manipulation**.  
- To understand **relationships** between entities (Employee & EmployeeDetail).  
- To solve **common interview questions** (Nth highest salary, joins, ratios, etc.).  
- To provide a **hands-on mini-project** for SQL learners.  

---

## 🔑 Key Points:-
- Two tables: **Employee** (personal data) and **EmployeeDetail** (work data).  
- Relationship: **One-to-Many** → One Employee can have multiple work records.  
- Uses **date formatting functions** (`STR_TO_DATE`) for correct date storage.  
- Includes **ER diagram** for schema visualization.  
- Covers **important SQL queries** (Joins, Aggregations, Ranking).  

---

## 📊 Key Insights
- Helps analyze employee data like **gender ratio, salary distribution, joining year trends**.  
- Demonstrates **data masking** (salary masking for security).  
- Shows **Nth highest salary** retrieval using:
  - Subqueries  
  - `LIMIT / OFFSET`  
  - `DENSE_RANK()` window function  
- Useful for **interview preparation** and **database learning projects**.  

---

## 🏗️ Database Schema

### 1. Employee Table
```sql
CREATE TABLE Employee (
    EmpID INT NOT NULL,
    EmpName VARCHAR(50),
    Gender CHAR,
    Salary INT,
    City CHAR(20)
);
