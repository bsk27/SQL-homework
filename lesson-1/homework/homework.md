# Lesson 1: Introduction to SQL Server and SSMS

> **Notes before doing the tasks:**
> - Tasks should be solved using **SQL Server**.
> - Case insensitivity applies.
> - Alias names do not affect the score.
> - Scoring is based on the **correct output**.
> - One correct solution is sufficient.

## Easy
1. Define the following terms: data, database, relational database, and table. 
2. List five key features of SQL Server.
3. What are the different authentication modes available when connecting to SQL Server? (Give at least 2)

1. Data is information in its raw form. It can be numbers, words, pictures, or sounds. Data by itself, it's not very useful, but when organized, it can help us understand things, events and behaviors
database is like a digital filing cabinet. It's a place to store data in an organized way, so we can easily find, use, or change it later
relational database stores data in tables, like a spreadsheet linked to each other, so we can combine data from different places, as we use any cell to relate to its respective ID “primary key”
table is part of a database, consist of rows and columns, each row is a record (like one person or item), and each column holds a type of information (like a name or age, gender, cost of item)

2. Here is five key feauters of SQL Server: 
1.Relational Database Engine stores data in tables and lets us query it using SQL.
2.High Availability keeps the database running with backup and failover features
3.Security protects data with encryption, access controls, and masking using login and password to enter, we can only get data using SQL queries 
4.Business Intelligence helps with reporting, data integration, and analysis
5.Performance optimizes speed with indexing, in-memory storage

3. Windows Authentication uses your Windows login; more secure and managed by the system.
SQL Server Authentication uses a separate username and password set in SQL Server; good for non-Windows access. SQL Server can be configured to allow both modes simultaneously (Mixed Mode Authentication).



## Medium
4. Create a new database in SSMS named SchoolDB.
5. Write and execute a query to create a table called Students with columns: StudentID (INT, PRIMARY KEY), Name (VARCHAR(50)), Age (INT).
6. Describe the differences between SQL Server, SSMS, and SQL.

4-5. Query that is used to creat the table: 
CREATE TABLE Students (
    StudentID INT PRIMARY KEY,
    Name VARCHAR(50),
    Age INT
);

![image](https://github.com/user-attachments/assets/cca0b2b7-3347-4a99-8218-cd66984f88ef)

6. SQL Server is a Database Management System (DBMS) created by Microsoft to 
store data, runs SQL commands, ensures the data is safe, fast to access, and well-organized

SSMS is a tool that helps to work with SQL Server more easily.
With SSMS, we can:
Write and run SQL queries
Create databases and tables
View and edit data in a friendly UI
Manage users, backups, and more

SQL is used to:
Create tables (CREATE TABLE)
Insert data (INSERT INTO)
Get data (SELECT)
Update data (UPDATE)
Delete data (DELETE)


## Hard
7. Research and explain the different SQL commands: DQL, DML, DDL, DCL, TCL with examples.
8. Write a query to insert three records into the Students table.
9. Restore AdventureWorksDW2022.bak file to your server. (write its steps to submit)
   You can find the database from this link :`https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorksDW2022.bak`

7.DQL used to query data from the database and to retrive data from tables. Usually the command SELECT is used.
DML is used to insert, update and delete data inside tables keeping the structure of the table unchanged, usually we use the following commands: INSERT, UPDATE, DELETE.
DDL used to create, add and delete column to the tables, also modify tables and databases.
DCL used to permit users to allow or disallow them to access and/or modify data 
TCL used to control how DML quearies are done to manage transactions (i.e. bundles of DML queries).


8. I used the following commands to insert 3 records into the table: 
![image](https://github.com/user-attachments/assets/11ee672d-c7f4-43a6-b8d1-804b23fa6971)

9. I followed the windows below, to restore the .bak database:

![image](https://github.com/user-attachments/assets/d1a6151c-54bd-49b4-95f5-e85c5e78a48a)
![image](https://github.com/user-attachments/assets/c77efbcf-fa63-4dea-a0d6-ab2ecbed40d5)

