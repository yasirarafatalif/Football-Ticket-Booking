# 🎟️ Football Ticket Booking Management System (SQL)

## 📌 Project Overview

This project is a simple **Football Ticket Booking Management System** built using **PostgreSQL**. It demonstrates database design, table relationships, constraints, and SQL queries for managing football matches, users, and ticket bookings.

---

## 🛠️ Technologies Used

* PostgreSQL
* SQL

---

## 📂 Database Tables

The project contains three tables:

### 1. Users

Stores information about users.

**Columns:**

* user_id (Primary Key)
* full_name
* email (Unique)
* role
* phone_number

---

### 2. Matches

Stores football match information.

**Columns:**

* match_id (Primary Key)
* fixture
* tournament_category
* base_ticket_price
* match_status

---

### 3. Bookings

Stores ticket booking information.

**Columns:**

* booking_id (Primary Key)
* user_id (Foreign Key)
* match_id (Foreign Key)
* seat_number
* payment_status
* total_cost

---

## 🔗 Relationships

* One **User** can have multiple **Bookings**.
* One **Match** can have multiple **Bookings**.
* **Bookings** connects the **Users** and **Matches** tables using foreign keys.

---

## ✨ SQL Features Used

* CREATE TABLE
* PRIMARY KEY
* FOREIGN KEY
* CHECK Constraint
* UNIQUE Constraint
* DROP TABLE
* SELECT
* WHERE
* ILIKE
* COALESCE
* INNER JOIN
* LEFT JOIN
* Subquery
* AVG()
* ROUND()
* ORDER BY
* LIMIT

---

## 📋 Queries Included

* Find all available Champions League matches.
* Search users by name using `ILIKE`.
* Replace NULL payment status using `COALESCE`.
* Retrieve booking details with user and match information using `INNER JOIN`.
* Display all users with or without bookings using `LEFT JOIN`.
* Find bookings whose total cost is greater than the average booking cost.
* Retrieve the top 2 most expensive matches.

---

## ▶️ How to Run

1. Open PostgreSQL or pgAdmin.
2. Create a new database.
3. Execute the SQL script.
4. Run the SELECT queries to view the results.

---

## 📖 Learning Objectives

This project demonstrates:

* Database design
* Table relationships
* Constraints
* Joins
* Aggregate Functions
* Subqueries
* Data Filtering
* SQL Best Practices

---

## 👨‍💻 Author

**Yasir Arafat Alif**

Dhaka Polytechnic Institute
Computer Science & Technology (CST)
