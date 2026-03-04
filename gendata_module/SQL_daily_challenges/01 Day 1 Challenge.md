## Determine the difference between SQL and No-SQL.

In subsequent days, you will be practising SQL Queries, but first you need to understand the fundamentals of Relational and Non Relational Databases. 

You can find the SQL queries related project description and starter code on GitHub Classroom through this link:  
[https://classroom.github.com/a/2rSN6arA](https://classroom.github.com/a/2rSN6arA)

**NOTE:** For the challenges listed, you will be not be expected to submit your codes, instead the technical mentor will share the solutions for the SQL related questions by the end of the week. 

For Day 1, you are expected to write, in your markdown, at least 5 differences between SQL and No-SQL Databases. 

## SQL Table Constraints and Database Creation

You have learnt about SQL Table Constraints. You are going to create 4 tables to store your data. 

You own a business called **ABC**. To drive dependable decisions using data, you will develop an SQL database, call it **ABC_DATA**, which you will use to store all your **customer info**, **customer orders**, **product info**, and your **order information**.

> **NB:** If you are using Google Collab for your queries, you are advised not to submit your answers in chunks. Instead, after the **Day 5 Challenge**, you can upload your final notebook to your GitHub Repository. 

---

## In these series of challenges, in SQL you are going to do the following:

- Create a database and name it `ABC_DATA`.
- Create 4 tables, in which you will insert the following datapoints:

---

### 1.1 customers Example Data:

| customer_id | first_name | last_name | email               |
|-------------|------------|-----------|---------------------|
| 1           | Joe        | Doe       | johndoe@email.com   |

---

### 1.2 products Example Data:

| product_id | product_name | price |
|------------|--------------|-------|
| 1          | Product A    | 10.00 |

---

### 1.3 orders Example Data:

| order_id | customer_id | order_date  |
|----------|-------------|-------------|
| 1        | 1           | 2023-05-01  |

---

### 1.4 order_items Example Data:

| order_id | product_id | quantity |
|----------|------------|----------|
| 1        | 1          | 2        |

---

### Example: Your queries will have the following syntax

```sql
CREATE TABLE students (
  student_id integer PRIMARY KEY,
  student_first_name varchar(100),
  student_last_name varchar(100),
  student_email varchar(100)
);
