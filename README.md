# Sql Tribe Block
# SQL Tutorial 🗄️

SQL (Structured Query Language) is used to manage and manipulate relational databases.

## 📚 Topics Covered
1. [Introduction to SQL](#introduction-to-sql)
2. [Database & Tables](#database--tables)
3. [CRUD Operations](#crud-operations)
4. [Filtering with WHERE](#filtering-with-where)
5. [Sorting and Aggregation](#sorting-and-aggregation)
6. [Joins](#joins)
7. [Indexes & Optimization](#indexes--optimization)

---

## 1. Introduction to SQL  
SQL is used to interact with databases like MySQL, PostgreSQL, SQLite, and SQL Server.

## 2. Database & Tables  
### Creating a Database  
```sql
CREATE DATABASE mydatabase;
```
## Creating a Table
```sql
CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(50),
    email VARCHAR(100) UNIQUE
);
```
## 3. CRUD Operations
```sql
INSERT INTO users (name, email) VALUES ('John Doe', 'john@example.com');
```
## Read Data
```sql
SELECT * FROM users;
```
## Update Data
```sql
UPDATE users SET name = 'Jane Doe' WHERE id = 1;
```
## Delete Data
```sql
DELETE FROM users WHERE id = 1;
```
## 4. Filtering with WHERE
```sql
SELECT * FROM users WHERE email = 'john@example.com';
```
## 5. Sorting and Aggregation
```sql
SELECT name, COUNT(*) FROM users GROUP BY name ORDER BY COUNT(*) DESC;
```
## 6. Joins
```sql
SELECT users.name, orders.amount 
FROM users 
JOIN orders ON users.id = orders.user_id;
```
## 7. Indexes & Optimization
```sql
CREATE INDEX idx_email ON users(email);
```
# 🌐 Further Reading
* [SQL Tutorial - W3Schools](https://www.w3schools.com/sql/)
* [MySQL Official Documentation](https://dev.mysql.com/doc/)
