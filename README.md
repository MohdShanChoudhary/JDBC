## MySQL Setup Instructions for JDBC Project

To set up the database for your JDBC-based Java application, follow these simple steps to create the required database and table in MySQL.

## Step 1: Open MySQL

Use one of the following:





MySQL Terminal (Command Line)



MySQL Workbench

## Step 2: Create the Database

CREATE DATABASE jdbc;

## Step 3: Switch to the Database

USE jdbc;

## Step 4: Create the Table

CREATE TABLE data (
    name VARCHAR(225),
    id INT PRIMARY KEY,
    num DECIMAL(10,0)
);

Table Columns:





name: Stores a person's name



id: Primary key (must be unique)



num: Stores a number (e.g., phone number)

## Step 5: (Optional) Insert Sample Data

INSERT INTO data (name, id, num) VALUES 
('Shan', 1, 9876543210),
('Ali', 2, 9123456789),
('Zara', 3, 9988776655);

Step 6: Verify the Data

SELECT * FROM data;

Expected Output:

## +-------+----+------------+
## | name  | id |    num     |
## +-------+----+------------+
## | Shan  |  1 | 9876543210 |
## | Ali   |  2 | 9123456789 |
## | Zara  |  3 | 9988776655 |
## +-------+----+------------+
