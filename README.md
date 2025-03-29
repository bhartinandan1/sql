# SQL

## Introduction to SQL

SQL, or Structured Query Language, is a standardized programming language used to manage and manipulate relational databases. It is the foundation for interacting with databases, allowing users to perform a variety of operations such as querying, updating, and managing data.

### Why Do We Need SQL?

Databases are essential for storing and organizing data in a structured manner. SQL provides a powerful and efficient way to interact with these databases. Here are some key reasons why SQL is important:

1. **Data Retrieval**  
    SQL enables users to retrieve specific data from large datasets using queries. For example, you can fetch all employees in a specific department or find customers who made purchases in the last month.

2. **Data Manipulation**  
    SQL allows users to insert, update, and delete data in a database. This makes it easy to keep the database up-to-date and accurate.

3. **Data Definition**  
    SQL provides commands to define and modify the structure of a database, such as creating tables, altering columns, and setting constraints.

4. **Data Control**  
    SQL includes features for controlling access to data, ensuring that only authorized users can perform specific operations.

5. **Standardized Language**  
    SQL is a widely adopted standard, supported by most relational database management systems (RDBMS) like MySQL, PostgreSQL, SQL Server, and Oracle. This makes it a universal tool for database management.

6. **Scalability and Performance**  
    SQL is optimized for handling large volumes of data efficiently, making it suitable for applications ranging from small-scale projects to enterprise-level systems.

### Key Features of SQL

- **Declarative Syntax**: SQL allows users to specify what they want to do with the data without worrying about how the database will execute the operation.
- **Portability**: SQL can be used across different platforms and database systems with minimal changes.
- **Extensibility**: SQL supports advanced features like stored procedures, triggers, and views to enhance functionality.

### Common SQL Commands

SQL commands are categorized into the following groups:

1. **Data Query Language (DQL)**  
    - `SELECT`: Used to retrieve data from a database.

2. **Data Definition Language (DDL)**  
    - `CREATE`, `ALTER`, `DROP`: Used to define and modify database structures.

3. **Data Manipulation Language (DML)**  
    - `INSERT`, `UPDATE`, `DELETE`: Used to manipulate data within tables.

4. **Data Control Language (DCL)**  
    - `GRANT`, `REVOKE`: Used to control access to data.

5. **Transaction Control Language (TCL)**  
    - `COMMIT`, `ROLLBACK`, `SAVEPOINT`: Used to manage database transactions.

### Conclusion

SQL is an indispensable tool for working with relational databases. Its versatility, efficiency, and ease of use make it a critical skill for developers, data analysts, and database administrators. Whether you're building a small application or managing a large enterprise system, SQL provides the foundation for effective data management.

## How to Install MySQL: Step-by-Step Guide

Installing MySQL involves downloading the software, setting it up, and configuring it for use. Follow these steps to install MySQL on your system:

### Step 1: Download MySQL
1. Visit the [MySQL Community Downloads](https://dev.mysql.com/downloads/) page.
2. Select the appropriate version for your operating system (Windows, macOS, or Linux).
3. Download the MySQL Installer or the required package.

### Step 2: Install MySQL on Your System
#### For Windows:
1. Run the downloaded MySQL Installer.
2. Choose the setup type:
    - **Developer Default**: Installs MySQL Server, MySQL Workbench, and other tools.
    - **Server Only**: Installs only the MySQL Server.
    - **Custom**: Allows you to select specific components.
3. Follow the on-screen instructions to proceed with the installation.

#### For macOS:
1. Open the downloaded `.dmg` file.
2. Follow the installation wizard to install MySQL.
3. After installation, start MySQL from **System Preferences**.

#### For Linux:
1. Use your package manager to install MySQL. For example:
    ```bash
    sudo apt update
    sudo apt install mysql-server
    ```
2. Start the MySQL service:
    ```bash
    sudo systemctl start mysql
    ```

### Step 3: Configure MySQL
1. During installation, you may be prompted to set a root password. Choose a strong password and remember it.
2. Configure the server settings as needed (e.g., port number, authentication method).
3. Complete the configuration and finish the installation.

### Step 4: Verify the Installation
1. Open a terminal or command prompt.
2. Run the following command to log in to MySQL:
    ```bash
    mysql -u root -p
    ```
3. Enter the root password you set during installation. If successful, you will see the MySQL prompt.

### Step 5: Optional Tools
- **MySQL Workbench**: A graphical tool for managing MySQL databases.
- **MySQL Shell**: An advanced command-line interface for MySQL.

### Conclusion
By following these steps, you can successfully install and configure MySQL on your system. Once installed, you can start creating databases, running queries, and managing your data.

## Types of SQL Commands

SQL commands are categorized based on their functionality. Here are the main types:

1. **Data Query Language (DQL)**  
    - Used to retrieve data from a database.
    - Example: `SELECT`

2. **Data Definition Language (DDL)**  
    - Used to define and manage database structures.
    - Examples: `CREATE`, `ALTER`, `DROP`, `TRUNCATE`

3. **Data Manipulation Language (DML)**  
    - Used to manipulate data within tables.
    - Examples: `INSERT`, `UPDATE`, `DELETE`

4. **Data Control Language (DCL)**  
    - Used to control access to data.
    - Examples: `GRANT`, `REVOKE`

5. **Transaction Control Language (TCL)**  
    - Used to manage database transactions.
    - Examples: `COMMIT`, `ROLLBACK`, `SAVEPOINT`

### Summary Table

| Command Type | Purpose                          | Examples                     |
|--------------|----------------------------------|------------------------------|
| DQL          | Query data                      | `SELECT`                     |
| DDL          | Define database structures      | `CREATE`, `ALTER`, `DROP`    |
| DML          | Manipulate data                 | `INSERT`, `UPDATE`, `DELETE` |
| DCL          | Control access                  | `GRANT`, `REVOKE`            |
| TCL          | Manage transactions             | `COMMIT`, `ROLLBACK`         |

### Conclusion

Understanding the types of SQL commands is crucial for effectively interacting with databases. Each category serves a specific purpose, enabling you to perform a wide range of operations.

## Databases and Related SQL Commands

A **database** is an organized collection of data that can be easily accessed, managed, and updated. Databases are essential for storing information in a structured format, enabling efficient data retrieval and manipulation.

### Types of Databases

1. **Relational Databases**  
    - Store data in tables with rows and columns.
    - Use SQL for querying and managing data.
    - Examples: MySQL, PostgreSQL, Oracle, SQL Server.

2. **NoSQL Databases**  
    - Designed for unstructured or semi-structured data.
    - Do not rely on fixed table schemas.
    - Examples: MongoDB, Cassandra, Redis.

3. **In-Memory Databases**  
    - Store data in memory for faster access.
    - Examples: Redis, Memcached.

4. **Cloud Databases**  
    - Hosted on cloud platforms for scalability and accessibility.
    - Examples: Amazon RDS, Google Cloud SQL, Azure SQL Database.

### Common SQL Commands for Databases

1. **Creating a Database**  
    ```sql
    CREATE DATABASE DatabaseName;
    ```

2. **Using a Database**  
    ```sql
    USE DatabaseName;
    ```

3. **Creating a Table**  
    ```sql
    CREATE TABLE TableName (
         Column1 DataType Constraints,
         Column2 DataType Constraints,
         ...
    );
    ```

4. **Inserting Data into a Table**  
    ```sql
    INSERT INTO TableName (Column1, Column2, ...)
    VALUES (Value1, Value2, ...);
    ```

5. **Querying Data**  
    ```sql
    SELECT Column1, Column2, ...
    FROM TableName
    WHERE Condition;
    ```

6. **Updating Data**  
    ```sql
    UPDATE TableName
    SET Column1 = Value1, Column2 = Value2, ...
    WHERE Condition;
    ```

7. **Deleting Data**  
    ```sql
    DELETE FROM TableName
    WHERE Condition;
    ```

8. **Dropping a Table**  
    ```sql
    DROP TABLE TableName;
    ```

9. **Dropping a Database**  
    ```sql
    DROP DATABASE DatabaseName;
    ```

### Example Workflow

1. **Create a Database**  
    ```sql
    CREATE DATABASE SchoolDB;
    ```

2. **Switch to the Database**  
    ```sql
    USE SchoolDB;
    ```

3. **Create a Table**  
    ```sql
    CREATE TABLE Students (
         StudentID INT PRIMARY KEY,
         Name VARCHAR(50),
         Age INT,
         Grade VARCHAR(10)
    );
    ```

4. **Insert Data into the Table**  
    ```sql
    INSERT INTO Students (StudentID, Name, Age, Grade)
    VALUES (1, 'John Doe', 15, '10th'),
             (2, 'Jane Smith', 16, '11th');
    ```

5. **Query the Data**  
    ```sql
    SELECT * FROM Students;
    ```

6. **Update a Record**  
    ```sql
    UPDATE Students
    SET Grade = '12th'
    WHERE StudentID = 2;
    ```

7. **Delete a Record**  
    ```sql
    DELETE FROM Students
    WHERE StudentID = 1;
    ```

### Conclusion

Databases are the backbone of modern applications, and SQL provides the tools to interact with them effectively. By mastering SQL commands, you can create, manage, and manipulate databases to meet your application's needs.

## SQL Commands for Table Management

Tables are fundamental components of a relational database. Below are some common SQL commands for creating, modifying, and managing tables.

### Creating a Table
To create a new table in a database:
```sql
CREATE TABLE TableName (
    Column1 DataType Constraints,
    Column2 DataType Constraints,
    ...
);
```

**Example:**
```sql
CREATE TABLE Employees (
    EmployeeID INT PRIMARY KEY,
    Name VARCHAR(50) NOT NULL,
    Department VARCHAR(50),
    Salary DECIMAL(10, 2)
);
```

### Altering a Table
To modify an existing table:
- **Add a Column:**
    ```sql
    ALTER TABLE TableName
    ADD ColumnName DataType Constraints;
    ```

    **Example:**
    ```sql
    ALTER TABLE Employees
    ADD HireDate DATE;
    ```

- **Modify a Column:**
    ```sql
    ALTER TABLE TableName
    MODIFY ColumnName NewDataType;
    ```

    **Example:**
    ```sql
    ALTER TABLE Employees
    MODIFY Salary DECIMAL(12, 2);
    ```

- **Drop a Column:**
    ```sql
    ALTER TABLE TableName
    DROP COLUMN ColumnName;
    ```

    **Example:**
    ```sql
    ALTER TABLE Employees
    DROP COLUMN HireDate;
    ```

### Dropping a Table
To delete a table and all its data:
```sql
DROP TABLE TableName;
```

**Example:**
```sql
DROP TABLE Employees;
```

### Renaming a Table
To rename an existing table:
```sql
RENAME TABLE OldTableName TO NewTableName;
```

**Example:**
```sql
RENAME TABLE Employees TO Staff;
```

### Truncating a Table
To remove all rows from a table without deleting the table structure:
```sql
TRUNCATE TABLE TableName;
```

**Example:**
```sql
TRUNCATE TABLE Employees;
```

### Viewing Table Structure
To view the structure of a table:
```sql
DESCRIBE TableName;
```

**Example:**
```sql
DESCRIBE Employees;
```

### Example Workflow
1. **Create a Table:**
    ```sql
    CREATE TABLE Products (
        ProductID INT PRIMARY KEY,
        ProductName VARCHAR(100),
        Price DECIMAL(10, 2),
        Stock INT
    );
    ```

2. **Add a Column:**
    ```sql
    ALTER TABLE Products
    ADD Category VARCHAR(50);
    ```

3. **Modify a Column:**
    ```sql
    ALTER TABLE Products
    MODIFY Price DECIMAL(12, 2);
    ```

4. **Drop a Column:**
    ```sql
    ALTER TABLE Products
    DROP COLUMN Stock;
    ```

5. **Rename the Table:**
    ```sql
    RENAME TABLE Products TO Inventory;
    ```

6. **Truncate the Table:**
    ```sql
    TRUNCATE TABLE Inventory;
    ```

7. **Drop the Table:**
    ```sql
    DROP TABLE Inventory;
    ```

### Conclusion
These commands allow you to create, modify, and manage tables effectively, ensuring your database structure meets your application's requirements.

## Building a Database: From Table Creation to Filling Data

Creating a database involves several steps, from defining the database structure to populating it with data. Below is a step-by-step guide with examples.

### Step 1: Create a Database
Start by creating a new database to store your tables.

```sql
CREATE DATABASE LibraryDB;
```

Switch to the newly created database:

```sql
USE LibraryDB;
```

### Step 2: Create a Table
Define the structure of a table to store data. For example, a table for books in a library:

```sql
CREATE TABLE Books (
    BookID INT PRIMARY KEY,
    Title VARCHAR(100) NOT NULL,
    Author VARCHAR(100),
    Genre VARCHAR(50),
    PublishedYear INT,
    CopiesAvailable INT
);
```

### Step 3: Insert Data into the Table
Add records to the table using the `INSERT INTO` statement.

```sql
INSERT INTO Books (BookID, Title, Author, Genre, PublishedYear, CopiesAvailable)
VALUES 
(1, 'To Kill a Mockingbird', 'Harper Lee', 'Fiction', 1960, 5),
(2, '1984', 'George Orwell', 'Dystopian', 1949, 3),
(3, 'The Great Gatsby', 'F. Scott Fitzgerald', 'Classic', 1925, 4),
(4, 'The Catcher in the Rye', 'J.D. Salinger', 'Fiction', 1951, 2);
```

### Step 4: Query the Data
Retrieve data from the table to verify the records.

```sql
SELECT * FROM Books;
```

**Result:**

| BookID | Title                   | Author             | Genre      | PublishedYear | CopiesAvailable |
|--------|-------------------------|--------------------|------------|---------------|-----------------|
| 1      | To Kill a Mockingbird   | Harper Lee         | Fiction    | 1960          | 5               |
| 2      | 1984                    | George Orwell      | Dystopian  | 1949          | 3               |
| 3      | The Great Gatsby        | F. Scott Fitzgerald| Classic    | 1925          | 4               |
| 4      | The Catcher in the Rye  | J.D. Salinger      | Fiction    | 1951          | 2               |

### Step 5: Update Data
Modify existing records in the table.

```sql
UPDATE Books
SET CopiesAvailable = 6
WHERE BookID = 1;
```

### Step 6: Delete Data
Remove specific records from the table.

```sql
DELETE FROM Books
WHERE BookID = 4;
```

### Step 7: Drop the Table (Optional)
If you no longer need the table, you can delete it.

```sql
DROP TABLE Books;
```

### Conclusion
By following these steps, you can create a database, define its structure, and populate it with data. This process is fundamental for managing and organizing information in any application.

## Data Types in SQL

Data types in SQL define the kind of data that can be stored in a column. Choosing the correct data type is essential for optimizing database performance and ensuring data integrity.

### Common SQL Data Types

1. **Numeric Data Types**  
    Used to store numbers.
    - `INT`: Integer values.
    - `DECIMAL(p, s)` or `NUMERIC(p, s)`: Fixed-point numbers with precision `p` and scale `s`.
    - `FLOAT` or `REAL`: Approximate floating-point numbers.

    **Example:**
    ```sql
    CREATE TABLE Products (
        ProductID INT PRIMARY KEY,
        Price DECIMAL(10, 2),
        Stock INT
    );
    ```

2. **Character/String Data Types**  
    Used to store text.
    - `CHAR(n)`: Fixed-length string of `n` characters.
    - `VARCHAR(n)`: Variable-length string with a maximum of `n` characters.
    - `TEXT`: Large text data.

    **Example:**
    ```sql
    CREATE TABLE Customers (
        CustomerID INT PRIMARY KEY,
        Name VARCHAR(50),
        Address TEXT
    );
    ```

3. **Date and Time Data Types**  
    Used to store date and time values.
    - `DATE`: Stores only the date (e.g., `YYYY-MM-DD`).
    - `TIME`: Stores only the time (e.g., `HH:MM:SS`).
    - `DATETIME`: Stores both date and time.
    - `TIMESTAMP`: Stores date and time with time zone information.

    **Example:**
    ```sql
    CREATE TABLE Orders (
        OrderID INT PRIMARY KEY,
        OrderDate DATE,
        DeliveryTime TIME,
        CreatedAt DATETIME
    );
    ```

4. **Boolean Data Type**  
    Used to store `TRUE` or `FALSE` values.
    - `BOOLEAN`: Typically stored as `1` (TRUE) or `0` (FALSE).

    **Example:**
    ```sql
    CREATE TABLE Features (
        FeatureID INT PRIMARY KEY,
        IsActive BOOLEAN
    );
    ```

5. **Binary Data Types**  
    Used to store binary data such as images or files.
    - `BLOB`: Binary Large Object.
    - `VARBINARY(n)`: Variable-length binary data.

    **Example:**
    ```sql
    CREATE TABLE Files (
        FileID INT PRIMARY KEY,
        FileData BLOB
    );
    ```

6. **Other Data Types**  
    - `ENUM`: A predefined list of values.
    - `SET`: A collection of predefined values.

    **Example:**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Role ENUM('Manager', 'Developer', 'Analyst')
    );
    ```

### Example Table with Various Data Types

```sql
CREATE TABLE ExampleTable (
    ID INT PRIMARY KEY,
    Name VARCHAR(100),
    Age INT,
    Salary DECIMAL(10, 2),
    JoinDate DATE,
    IsPermanent BOOLEAN
);
```

### Conclusion

Understanding SQL data types is crucial for designing efficient and reliable databases. By selecting appropriate data types, you can ensure data accuracy and optimize storage.

## Keys in SQL

Keys in SQL are attributes or sets of attributes that help uniquely identify rows in a table. They play a crucial role in maintaining data integrity and establishing relationships between tables.

### Types of Keys in SQL

1. **Primary Key**  
    - Uniquely identifies each record in a table.
    - Cannot contain `NULL` values.
    - A table can have only one primary key.

    **Example:**
    ```sql
    CREATE TABLE Students (
        StudentID INT PRIMARY KEY,
        Name VARCHAR(50),
        Age INT
    );
    ```

2. **Foreign Key**  
    - Establishes a relationship between two tables.
    - Refers to the primary key in another table.
    - Ensures referential integrity.

    **Example:**
    ```sql
    CREATE TABLE Orders (
        OrderID INT PRIMARY KEY,
        CustomerID INT,
        FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID)
    );
    ```

3. **Unique Key**  
    - Ensures all values in a column are unique.
    - Allows one `NULL` value (depending on the database system).

    **Example:**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Email VARCHAR(100) UNIQUE
    );
    ```

4. **Candidate Key**  
    - A set of attributes that can uniquely identify a record.
    - A table can have multiple candidate keys, but only one can be chosen as the primary key.

    **Example:**
    In a `Students` table, both `StudentID` and `Email` could be candidate keys.

5. **Composite Key**  
    - A key made up of two or more columns to uniquely identify a record.
    - Used when a single column is not sufficient to ensure uniqueness.

    **Example:**
    ```sql
    CREATE TABLE Enrollments (
        StudentID INT,
        CourseID INT,
        PRIMARY KEY (StudentID, CourseID)
    );
    ```

6. **Super Key**  
    - A set of attributes that can uniquely identify a record.
    - Includes primary keys and candidate keys.

    **Example:**
    In a `Books` table, `BookID` and `ISBN` together could form a super key.

7. **Alternate Key**  
    - Candidate keys that are not chosen as the primary key.
    - Acts as an alternative unique identifier.

    **Example:**
    If `StudentID` is the primary key, `Email` could be an alternate key.

### Importance of Keys in SQL

- **Uniqueness**: Ensure that each record in a table is unique.
- **Data Integrity**: Maintain consistency and accuracy of data.
- **Relationships**: Establish and enforce relationships between tables.
- **Indexing**: Improve query performance by creating indexes on keys.

### Example Workflow with Keys

1. **Create a Table with a Primary Key**  
    ```sql
    CREATE TABLE Departments (
        DepartmentID INT PRIMARY KEY,
        DepartmentName VARCHAR(50)
    );
    ```

2. **Add a Foreign Key**  
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Name VARCHAR(50),
        DepartmentID INT,
        FOREIGN KEY (DepartmentID) REFERENCES Departments(DepartmentID)
    );
    ```

3. **Insert Data**  
    ```sql
    INSERT INTO Departments (DepartmentID, DepartmentName)
    VALUES (1, 'HR'), (2, 'IT');

    INSERT INTO Employees (EmployeeID, Name, DepartmentID)
    VALUES (101, 'Alice', 1), (102, 'Bob', 2);
    ```

4. **Query Data with Relationships**  
    ```sql
    SELECT Employees.Name, Departments.DepartmentName
    FROM Employees
    JOIN Departments ON Employees.DepartmentID = Departments.DepartmentID;
    ```

### Conclusion

Keys are fundamental to database design, ensuring data integrity and enabling efficient data retrieval. By understanding and using keys effectively, you can create robust and well-structured databases.

## Constraints in SQL

Constraints in SQL are rules enforced on data in a table to ensure data integrity and accuracy. They define the valid data that can be stored in a column and help maintain the reliability of the database.

### Types of Constraints

1. **NOT NULL**  
    Ensures that a column cannot have `NULL` values.  
    **Example:**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Name VARCHAR(50) NOT NULL
    );
    ```

2. **UNIQUE**  
    Ensures that all values in a column are unique.  
    **Example:**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Email VARCHAR(100) UNIQUE
    );
    ```

3. **PRIMARY KEY**  
    Combines `NOT NULL` and `UNIQUE`. It uniquely identifies each record in a table.  
    **Example:**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Name VARCHAR(50)
    );
    ```

4. **FOREIGN KEY**  
    Establishes a relationship between two tables by referencing the primary key of another table.  
    **Example:**
    ```sql
    CREATE TABLE Orders (
        OrderID INT PRIMARY KEY,
        CustomerID INT,
        FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID)
    );
    ```

5. **CHECK**  
    Ensures that all values in a column satisfy a specific condition.  
    **Example:**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Age INT CHECK (Age >= 18)
    );
    ```

6. **DEFAULT**  
    Assigns a default value to a column if no value is provided.  
    **Example:**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Status VARCHAR(20) DEFAULT 'Active'
    );
    ```

7. **INDEX**  
    Improves the speed of data retrieval operations on a table.  
    **Example:**
    ```sql
    CREATE INDEX idx_name ON Employees (Name);
    ```

### Adding Constraints to Existing Tables

- **Add a NOT NULL Constraint:**
    ```sql
    ALTER TABLE Employees
    MODIFY Name VARCHAR(50) NOT NULL;
    ```

- **Add a UNIQUE Constraint:**
    ```sql
    ALTER TABLE Employees
    ADD CONSTRAINT unique_email UNIQUE (Email);
    ```

- **Add a CHECK Constraint:**
    ```sql
    ALTER TABLE Employees
    ADD CONSTRAINT check_age CHECK (Age >= 18);
    ```

- **Add a FOREIGN KEY Constraint:**
    ```sql
    ALTER TABLE Orders
    ADD CONSTRAINT fk_customer FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID);
    ```

### Dropping Constraints

- **Drop a UNIQUE Constraint:**
    ```sql
    ALTER TABLE Employees
    DROP CONSTRAINT unique_email;
    ```

- **Drop a CHECK Constraint:**
    ```sql
    ALTER TABLE Employees
    DROP CONSTRAINT check_age;
    ```

- **Drop a FOREIGN KEY Constraint:**
    ```sql
    ALTER TABLE Orders
    DROP CONSTRAINT fk_customer;
    ```

### Conclusion

Constraints are essential for maintaining data integrity and ensuring that the data stored in a database adheres to specific rules. By using constraints effectively, you can prevent invalid data from being entered into your tables.

## Foreign Key in SQL

A **foreign key** is a column or a set of columns in one table that establishes a link between the data in two tables. It refers to the `PRIMARY KEY` in another table, ensuring referential integrity by enforcing a relationship between the two tables.

### Key Features of a Foreign Key
1. Ensures that the value in the foreign key column matches a value in the referenced primary key column.
2. Prevents actions that would destroy the link between the two tables.
3. Can be used to enforce cascading updates or deletions.

### Syntax for Creating a Foreign Key
A foreign key is defined during table creation or added to an existing table.

#### During Table Creation
```sql
CREATE TABLE Orders (
    OrderID INT PRIMARY KEY,
    CustomerID INT,
    FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID)
);
```

#### Adding to an Existing Table
```sql
ALTER TABLE Orders
ADD CONSTRAINT fk_customer
FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID);
```

### Example: Foreign Key in Action

#### Step 1: Create the Parent Table
```sql
CREATE TABLE Customers (
    CustomerID INT PRIMARY KEY,
    Name VARCHAR(50),
    Email VARCHAR(100)
);
```

#### Step 2: Create the Child Table with a Foreign Key
```sql
CREATE TABLE Orders (
    OrderID INT PRIMARY KEY,
    CustomerID INT,
    OrderDate DATE,
    FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID)
);
```

#### Step 3: Insert Data into the Parent Table
```sql
INSERT INTO Customers (CustomerID, Name, Email)
VALUES 
(1, 'Alice', 'alice@example.com'),
(2, 'Bob', 'bob@example.com');
```

#### Step 4: Insert Data into the Child Table
```sql
INSERT INTO Orders (OrderID, CustomerID, OrderDate)
VALUES 
(101, 1, '2023-01-15'),
(102, 2, '2023-01-16');
```

### Cascading Actions with Foreign Keys

1. **ON DELETE CASCADE**  
   Automatically deletes rows in the child table when the corresponding row in the parent table is deleted.
   ```sql
   CREATE TABLE Orders (
       OrderID INT PRIMARY KEY,
       CustomerID INT,
       FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID) ON DELETE CASCADE
   );
   ```

2. **ON UPDATE CASCADE**  
   Automatically updates the foreign key in the child table when the primary key in the parent table is updated.
   ```sql
   CREATE TABLE Orders (
       OrderID INT PRIMARY KEY,
       CustomerID INT,
       FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID) ON UPDATE CASCADE
   );
   ```

### Querying Data with Foreign Keys
To retrieve data from related tables, use a `JOIN`:
```sql
SELECT Orders.OrderID, Customers.Name, Orders.OrderDate
FROM Orders
JOIN Customers ON Orders.CustomerID = Customers.CustomerID;
```

### Conclusion
Foreign keys are essential for maintaining relationships between tables and ensuring data integrity. By using foreign keys, you can enforce rules that preserve the consistency and reliability of your database.

## UPDATE Command in SQL

The `UPDATE` command in SQL is used to modify existing records in a table. It allows you to update one or more columns for one or more rows based on a specified condition.

### Syntax
```sql
UPDATE TableName
SET Column1 = Value1, Column2 = Value2, ...
WHERE Condition;
```

- `TableName`: The name of the table where the update will occur.
- `SET`: Specifies the column(s) to update and their new values.
- `WHERE`: Specifies the condition to identify which rows to update. If omitted, all rows in the table will be updated.

### Example: Updating a Single Row
```sql
UPDATE Employees
SET Salary = 55000
WHERE EmployeeID = 1;
```
This updates the `Salary` of the employee with `EmployeeID` 1 to 55000.

### Example: Updating Multiple Rows
```sql
UPDATE Employees
SET Department = 'HR'
WHERE Department = 'Human Resources';
```
This updates all rows where the `Department` is "Human Resources" to "HR".

### Example: Updating Multiple Columns
```sql
UPDATE Employees
SET Salary = 60000, Department = 'Finance'
WHERE EmployeeID = 2;
```
This updates the `Salary` and `Department` of the employee with `EmployeeID` 2.

### Updating All Rows
If no `WHERE` clause is specified, all rows in the table will be updated:
```sql
UPDATE Employees
SET Department = 'General';
```
This sets the `Department` of all employees to "General".

### Using Subqueries in UPDATE
You can use a subquery to update a column based on values from another table:
```sql
UPDATE Employees
SET Salary = (SELECT AVG(Salary) FROM Employees)
WHERE Department = 'IT';
```
This sets the `Salary` of all employees in the "IT" department to the average salary of all employees.

### Precautions
- Always use the `WHERE` clause to avoid unintentionally updating all rows.
- Test your query with a `SELECT` statement before running the `UPDATE` command.

### Conclusion
The `UPDATE` command is a powerful tool for modifying data in a table. By using it carefully with conditions, you can ensure accurate and efficient updates to your database.

## DELETE Command in SQL

The `DELETE` command in SQL is used to remove rows from a table. It allows you to delete specific rows based on a condition or all rows if no condition is specified.

### Syntax
```sql
DELETE FROM TableName
WHERE Condition;
```

- `TableName`: The name of the table from which rows will be deleted.
- `WHERE`: Specifies the condition to identify which rows to delete. If omitted, all rows in the table will be deleted.

### Example: Deleting Specific Rows
```sql
DELETE FROM Employees
WHERE Department = 'HR';
```
This deletes all rows where the `Department` is "HR".

### Example: Deleting a Single Row
```sql
DELETE FROM Employees
WHERE EmployeeID = 1;
```
This deletes the row where the `EmployeeID` is 1.

### Deleting All Rows
If no `WHERE` clause is specified, all rows in the table will be deleted:
```sql
DELETE FROM Employees;
```
**Note:** The table structure remains intact, but all data is removed.

### Using Subqueries in DELETE
You can use a subquery to delete rows based on values from another table:
```sql
DELETE FROM Employees
WHERE DepartmentID IN (SELECT DepartmentID FROM Departments WHERE DepartmentName = 'Finance');
```

### Difference Between DELETE and TRUNCATE
- `DELETE`: Removes rows one by one and can include a `WHERE` clause. It logs each deletion and can be rolled back.
- `TRUNCATE`: Removes all rows from a table without logging individual row deletions. It cannot include a `WHERE` clause and is faster but cannot be rolled back.

### Precautions
- Always use the `WHERE` clause to avoid unintentionally deleting all rows.
- Test your query with a `SELECT` statement before running the `DELETE` command.

### Conclusion
The `DELETE` command is a powerful tool for removing data from a table. Use it carefully to ensure that only the intended rows are deleted.

## SELECT Command in SQL

The `SELECT` command in SQL is used to retrieve data from one or more tables in a database. It is one of the most commonly used SQL commands for querying data.

### Syntax
```sql
SELECT Column1, Column2, ...
FROM TableName
WHERE Condition;
```

- `Column1, Column2, ...`: The columns you want to retrieve.
- `TableName`: The name of the table from which to retrieve data.
- `WHERE`: Optional clause to filter rows based on a condition.

### Example: Basic SELECT Query
Retrieve all columns from the `Employees` table:
```sql
SELECT * FROM Employees;
```

### Example: Selecting Specific Columns
Retrieve only the `Name` and `Department` columns:
```sql
SELECT Name, Department FROM Employees;
```

### Using Aliases
You can use aliases to rename columns in the result set:
```sql
SELECT Name AS EmployeeName, Department AS Dept FROM Employees;
```

### Filtering Data with WHERE
Retrieve employees from the "IT" department:
```sql
SELECT * FROM Employees WHERE Department = 'IT';
```

### Sorting Data with ORDER BY
Retrieve employees sorted by `Salary` in descending order:
```sql
SELECT * FROM Employees ORDER BY Salary DESC;
```

### Limiting Results with LIMIT
Retrieve the top 5 highest-paid employees:
```sql
SELECT * FROM Employees ORDER BY Salary DESC LIMIT 5;
```

### Combining Conditions with AND/OR
Retrieve employees from the "IT" department with a salary greater than 50000:
```sql
SELECT * FROM Employees WHERE Department = 'IT' AND Salary > 50000;
```

### Using Aggregate Functions
Retrieve the total salary of all employees:
```sql
SELECT SUM(Salary) AS TotalSalary FROM Employees;
```

### Grouping Data with GROUP BY
Retrieve the total salary for each department:
```sql
SELECT Department, SUM(Salary) AS TotalSalary
FROM Employees
GROUP BY Department;
```

### Conclusion
The `SELECT` command is a versatile tool for querying data in SQL. By combining it with clauses like `WHERE`, `ORDER BY`, and `GROUP BY`, you can retrieve and analyze data effectively.

## WHERE Clause in SQL

The `WHERE` clause in SQL is used to filter records in a table based on specific conditions. It helps retrieve only the rows that meet the given criteria.

### Syntax
```sql
SELECT Column1, Column2, ...
FROM TableName
WHERE Condition;
```

### Example: Using the `WHERE` Clause

1. **Create a Table**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Name VARCHAR(50),
        Department VARCHAR(50),
        Salary INT
    );
    ```

2. **Insert Data**
    ```sql
    INSERT INTO Employees (EmployeeID, Name, Department, Salary)
    VALUES 
    (1, 'Alice', 'HR', 50000),
    (2, 'Bob', 'IT', 60000),
    (3, 'Charlie', 'Finance', 70000),
    (4, 'David', 'IT', 55000);
    ```

3. **Query with `WHERE`**
    - Retrieve employees from the "IT" department:
        ```sql
        SELECT * FROM Employees
        WHERE Department = 'IT';
        ```

        **Result:**
        ```
        EmployeeID | Name   | Department | Salary
        -----------------------------------------
        2          | Bob    | IT         | 60000
        4          | David  | IT         | 55000
        ```

    - Retrieve employees with a salary greater than 55000:
        ```sql
        SELECT * FROM Employees
        WHERE Salary > 55000;
        ```

        **Result:**
        ```
        EmployeeID | Name     | Department | Salary
        -------------------------------------------
        2          | Bob      | IT         | 60000
        3          | Charlie  | Finance    | 70000
        ```

    - Combine conditions using `AND`:
        ```sql
        SELECT * FROM Employees
        WHERE Department = 'IT' AND Salary > 55000;
        ```

        **Result:**
        ```
        EmployeeID | Name | Department | Salary
        ---------------------------------------
        2          | Bob  | IT         | 60000
        ```

    - Combine conditions using `OR`:
        ```sql
        SELECT * FROM Employees
        WHERE Department = 'HR' OR Salary > 60000;
        ```

        **Result:**
        ```
        EmployeeID | Name     | Department | Salary
        -------------------------------------------
        1          | Alice    | HR         | 50000
        3          | Charlie  | Finance    | 70000
        ```

### Conclusion

The `WHERE` clause is a simple yet powerful tool for filtering data in SQL. By using conditions like `=`, `>`, `<`, `AND`, and `OR`, you can retrieve only the rows that match your requirements.

## ALTER Command in SQL

The `ALTER` command in SQL is used to modify the structure of an existing table. It allows you to add, modify, or delete columns, as well as change table constraints.

### Syntax
```sql
ALTER TABLE TableName
ADD ColumnName DataType Constraints;

ALTER TABLE TableName
MODIFY ColumnName NewDataType;

ALTER TABLE TableName
DROP COLUMN ColumnName;
```

### Examples

1. **Add a Column**
    ```sql
    ALTER TABLE Employees
    ADD HireDate DATE;
    ```
    This adds a new column `HireDate` of type `DATE` to the `Employees` table.

2. **Modify a Column**
    ```sql
    ALTER TABLE Employees
    MODIFY Salary DECIMAL(12, 2);
    ```
    This changes the data type of the `Salary` column to `DECIMAL` with a precision of 12 and scale of 2.

3. **Drop a Column**
    ```sql
    ALTER TABLE Employees
    DROP COLUMN HireDate;
    ```
    This removes the `HireDate` column from the `Employees` table.

4. **Rename a Column** (Supported in some databases)
    ```sql
    ALTER TABLE Employees
    RENAME COLUMN OldColumnName TO NewColumnName;
    ```
    This renames a column in the table.

5. **Add a Constraint**
    ```sql
    ALTER TABLE Employees
    ADD CONSTRAINT unique_email UNIQUE (Email);
    ```
    This adds a `UNIQUE` constraint to the `Email` column.

6. **Drop a Constraint**
    ```sql
    ALTER TABLE Employees
    DROP CONSTRAINT unique_email;
    ```
    This removes the `UNIQUE` constraint from the `Email` column.

### Precautions
- Ensure you have a backup of the table before making structural changes.
- Be cautious when dropping columns or constraints, as it may lead to data loss or affect dependent queries.

### Conclusion
The `ALTER` command is a powerful tool for managing table structures in SQL. By using it effectively, you can adapt your database schema to meet changing requirements.

## RENAME Command in SQL

The `RENAME` command in SQL is used to change the name of a database object, such as a table. It allows you to rename an existing table to a new name.

### Syntax
```sql
RENAME TABLE OldTableName TO NewTableName;
```

- `OldTableName`: The current name of the table.
- `NewTableName`: The new name you want to assign to the table.

### Example: Renaming a Table

1. **Create a Table**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Name VARCHAR(50),
        Department VARCHAR(50)
    );
    ```

2. **Rename the Table**
    ```sql
    RENAME TABLE Employees TO Staff;
    ```

3. **Verify the Change**
    ```sql
    SHOW TABLES;
    ```

    **Result:**
    ```
    Tables_in_Database
    -------------------
    Staff
    ```

### Notes
- The `RENAME` command is not supported by all database systems. For example, in MySQL, you can use the `RENAME TABLE` statement, but in SQL Server, you need to use the `sp_rename` stored procedure.
- Ensure that no queries or operations are actively using the table when renaming it.

### Conclusion

The `RENAME` command is a simple and effective way to rename tables in SQL. It is particularly useful when you need to update table names to reflect changes in your database schema or application requirements.

## TRUNCATE Command in SQL

The `TRUNCATE` command in SQL is used to remove all rows from a table, effectively resetting it to an empty state. Unlike the `DELETE` command, `TRUNCATE` is faster and does not log individual row deletions, making it more efficient for large datasets.

### Syntax
```sql
TRUNCATE TABLE TableName;
```

- `TableName`: The name of the table you want to truncate.

### Key Features
1. **Removes All Rows**: Deletes all rows from the table.
2. **Resets Identity Columns**: Resets any auto-increment counters to their initial values.
3. **Faster than DELETE**: Does not log individual row deletions, making it faster for large tables.
4. **Cannot Be Rolled Back**: In most database systems, `TRUNCATE` is a non-transactional operation and cannot be undone.

### Example: Using TRUNCATE

1. **Create a Table**
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Name VARCHAR(50),
        Department VARCHAR(50),
        Salary INT
    );
    ```

2. **Insert Data**
    ```sql
    INSERT INTO Employees (EmployeeID, Name, Department, Salary)
    VALUES 
    (1, 'Alice', 'HR', 50000),
    (2, 'Bob', 'IT', 60000),
    (3, 'Charlie', 'Finance', 70000);
    ```

3. **Truncate the Table**
    ```sql
    TRUNCATE TABLE Employees;
    ```

4. **Verify the Table is Empty**
    ```sql
    SELECT * FROM Employees;
    ```

    **Result:**
    ```
    (No rows returned)
    ```

### Difference Between TRUNCATE and DELETE
| Feature               | TRUNCATE                          | DELETE                            |
|-----------------------|-----------------------------------|-----------------------------------|
| Removes All Rows      | Yes                               | Yes (if no `WHERE` clause)        |
| Logs Individual Rows  | No                                | Yes                               |
| Resets Identity Column| Yes                               | No                                |
| Rollback Support      | No (in most systems)              | Yes                               |
| Performance           | Faster                            | Slower for large datasets         |

### Precautions
- Use `TRUNCATE` only when you are sure you want to remove all rows from a table.
- Ensure you have a backup if the data is critical, as `TRUNCATE` cannot be rolled back in most systems.

### Conclusion
The `TRUNCATE` command is a powerful and efficient way to clear all data from a table while retaining its structure. It is particularly useful for resetting tables during development or maintenance tasks.

### Difference Between TRUNCATE, DELETE, and DROP Commands in SQL

When managing data in SQL, it's important to understand the differences between the `TRUNCATE`, `DELETE`, and `DROP` commands, as they serve distinct purposes and have different implications.

| Command   | Purpose                          | Can Use WHERE Clause? | Logs Individual Rows? | Resets Identity Columns? | Rollback Support | Deletes Table Structure? |
|-----------|----------------------------------|------------------------|------------------------|---------------------------|------------------|--------------------------|
| `TRUNCATE`| Removes all rows from a table    | No                     | No                     | Yes                       | No               | No                       |
| `DELETE`  | Removes specific rows from a table| Yes                    | Yes                    | No                        | Yes              | No                       |
| `DROP`    | Deletes the entire table         | No                     | No                     | N/A                       | No               | Yes                      |

### Key Differences

1. **TRUNCATE**  
    - Removes all rows from a table but retains the table structure.
    - Faster than `DELETE` as it does not log individual row deletions.
    - Resets identity columns (e.g., auto-increment values).
    - Cannot be rolled back in most database systems.

    **Example:**
    ```sql
    TRUNCATE TABLE Employees;
    ```

2. **DELETE**  
    - Removes specific rows based on a condition or all rows if no condition is provided.
    - Logs each row deletion, making it slower for large datasets.
    - Can be rolled back if used within a transaction.

    **Example:**
    ```sql
    DELETE FROM Employees WHERE Department = 'HR';
    ```

3. **DROP**  
    - Completely removes a table, including its structure and data.
    - Cannot be rolled back in most database systems.
    - Use with caution as it permanently deletes the table.

    **Example:**
    ```sql
    DROP TABLE Employees;
    ```

### When to Use Each Command

- Use `TRUNCATE` when you need to quickly clear all data from a table but keep its structure for future use.
- Use `DELETE` when you need to remove specific rows or when you want the option to roll back the operation.
- Use `DROP` when you no longer need the table and want to remove it entirely from the database.

### Conclusion

Understanding the differences between `TRUNCATE`, `DELETE`, and `DROP` is crucial for effective database management. Each command serves a specific purpose, and choosing the right one depends on your requirements and the impact on the database.


## DISTINCT Keyword in SQL

The `DISTINCT` keyword is used in SQL to remove duplicate values from the result set. It ensures that the query returns only unique values.

### Example: Using `DISTINCT` with a Database

Below is an example demonstrating the use of the `DISTINCT` keyword:

1. **Create a Database**  
    ```sql
    CREATE DATABASE CompanyDB;
    ```

2. **Use the Database**  
    ```sql
    USE CompanyDB;
    ```

3. **Create an Employee Table**  
    ```sql
    CREATE TABLE Employees (
        EmployeeID INT PRIMARY KEY,
        Name VARCHAR(50),
        Department VARCHAR(50),
        Salary INT
    );
    ```

4. **Insert Values into the Employee Table**  
    ```sql
    INSERT INTO Employees (EmployeeID, Name, Department, Salary)
    VALUES 
    (1, 'Alice', 'HR', 50000),
    (2, 'Bob', 'IT', 60000),
    (3, 'Charlie', 'HR', 50000),
    (4, 'David', 'Finance', 70000),
    (5, 'Eve', 'IT', 60000);
    ```

5. **Use the `DISTINCT` Keyword**  
    Retrieve unique departments from the `Employees` table:
    ```sql
    SELECT DISTINCT Department FROM Employees;
    ```

    **Result:**
    ```
    Department
    ----------
    HR
    IT
    Finance
    ```

6. **Another Example with Multiple Columns**  
    Retrieve unique combinations of `Department` and `Salary`:
    ```sql
    SELECT DISTINCT Department, Salary FROM Employees;
    ```

    **Result:**
    ```
    Department   | Salary
    ---------------------
    HR           | 50000
    IT           | 60000
    Finance      | 70000
    ```

### Conclusion

The `DISTINCT` keyword is a powerful tool for eliminating duplicate rows from query results. It is especially useful when working with large datasets where duplicate values might exist.

## SQL Operators

SQL operators are special keywords or symbols used to perform operations on data in a database. They are used in SQL queries to filter, compare, or manipulate data.

## Types of SQL Operators

1. **Arithmetic Operators**  
    Used to perform mathematical operations.
    - `+` (Addition)
    - `-` (Subtraction)
    - `*` (Multiplication)
    - `/` (Division)
    - `%` (Modulus)

    **Example:**
    ```sql
    SELECT 10 + 5 AS Addition, 10 - 5 AS Subtraction, 10 * 5 AS Multiplication, 10 / 5 AS Division;
    ```

2. **Comparison Operators**  
    Used to compare two values.
    - `=` (Equal)
    - `!=` or `<>` (Not Equal)
    - `>` (Greater Than)
    - `<` (Less Than)
    - `>=` (Greater Than or Equal To)
    - `<=` (Less Than or Equal To)

    **Example:**
    ```sql
    SELECT * FROM Employees WHERE Salary > 50000;
    ```

3. **Logical Operators**  
    Used to combine multiple conditions.
    - `AND`
    - `OR`
    - `NOT`

    **Example:**
    ```sql
    SELECT * FROM Employees WHERE Department = 'IT' AND Salary > 50000;
    ```

4. **Bitwise Operators**  
    Used to perform bit-level operations.
    - `&` (Bitwise AND)
    - `|` (Bitwise OR)
    - `^` (Bitwise XOR)

    **Example:**
    ```sql
    SELECT 5 & 3 AS BitwiseAND, 5 | 3 AS BitwiseOR, 5 ^ 3 AS BitwiseXOR;
    ```

5. **Set Operators**  
    Used to combine results of two or more queries.
    - `UNION`
    - `UNION ALL`
    - `INTERSECT`
    - `EXCEPT`

    **Example:**
    ```sql
    SELECT Name FROM Employees
    UNION
    SELECT Name FROM Managers;
    ```

6. **LIKE Operator**  
    Used for pattern matching with wildcards.
    - `%` (Matches zero or more characters)
    - `_` (Matches a single character)

    **Example:**
    ```sql
    SELECT * FROM Employees WHERE Name LIKE 'A%';
    ```

7. **IN Operator**  
    Used to specify multiple values in a `WHERE` clause.

    **Example:**
    ```sql
    SELECT * FROM Employees WHERE Department IN ('HR', 'IT', 'Finance');
    ```

8. **BETWEEN Operator**  
    Used to filter values within a range.

    **Example:**
    ```sql
    SELECT * FROM Employees WHERE Salary BETWEEN 30000 AND 60000;
    ```

9. **IS NULL Operator**  
    Used to check for `NULL` values.

    **Example:**
    ```sql
    SELECT * FROM Employees WHERE ManagerID IS NULL;
    ```

## Conclusion

SQL operators are essential for writing effective queries. By combining different operators, you can perform complex data manipulations and retrieve meaningful insights from your database.
