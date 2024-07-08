**Day 37: Exploring SQL – Quick Reference Guide**

On Day 37, I explored the SQL Quick Reference Guide from W3Schools. This guide provides a concise summary of essential SQL commands and functions, making it a valuable resource for quick look-ups and refreshing your knowledge. Let's dive into some of the key components covered in the SQL Quick Reference Guide with brief explanations.

**Key Components of the SQL Quick Reference Guide:**

1. **Data Types:**
   - Common data types include `INT`, `VARCHAR`, `DATE`, `FLOAT`, and `BOOLEAN`.
   - **Example:** `CREATE TABLE Students (ID INT, Name VARCHAR(50), EnrollmentDate DATE);`

2. **SQL Commands:**
   - **SELECT:** Retrieves data from a database.
     - **Example:** `SELECT * FROM Employees;`
   - **INSERT INTO:** Adds new rows to a table.
     - **Example:** `INSERT INTO Employees (Name, Age) VALUES ('John Doe', 30);`
   - **UPDATE:** Modifies existing data in a table.
     - **Example:** `UPDATE Employees SET Age = 31 WHERE Name = 'John Doe';`
   - **DELETE:** Removes rows from a table.
     - **Example:** `DELETE FROM Employees WHERE Name = 'John Doe';`

3. **Clauses:**
   - **WHERE:** Filters records based on a condition.
     - **Example:** `SELECT * FROM Employees WHERE Age > 30;`
   - **ORDER BY:** Sorts the result set.
     - **Example:** `SELECT * FROM Employees ORDER BY Age DESC;`
   - **GROUP BY:** Groups rows sharing a property.
     - **Example:** `SELECT Department, COUNT(*) FROM Employees GROUP BY Department;`
   - **HAVING:** Filters groups based on a condition.
     - **Example:** `SELECT Department, COUNT(*) FROM Employees GROUP BY Department HAVING COUNT(*) > 5;`

4. **Joins:**
   - Combines rows from two or more tables based on a related column.
   - **INNER JOIN:** Returns records with matching values in both tables.
     - **Example:** `SELECT Employees.Name, Departments.Department FROM Employees INNER JOIN Departments ON Employees.DepartmentID = Departments.ID;`
   - **LEFT JOIN:** Returns all records from the left table and matching records from the right table.
     - **Example:** `SELECT Employees.Name, Departments.Department FROM Employees LEFT JOIN Departments ON Employees.DepartmentID = Departments.ID;`
   - **RIGHT JOIN:** Returns all records from the right table and matching records from the left table.
     - **Example:** `SELECT Employees.Name, Departments.Department FROM Employees RIGHT JOIN Departments ON Employees.DepartmentID = Departments.ID;`
   - **FULL JOIN:** Returns records when there is a match in one of the tables.
     - **Example:** `SELECT Employees.Name, Departments.Department FROM Employees FULL JOIN Departments ON Employees.DepartmentID = Departments.ID;`

5. **Aggregate Functions:**
   - **SUM():** Returns the total sum of a numeric column.
     - **Example:** `SELECT SUM(Salary) FROM Employees;`
   - **AVG():** Returns the average value of a numeric column.
     - **Example:** `SELECT AVG(Salary) FROM Employees;`
   - **COUNT():** Returns the number of rows that match a specified condition.
     - **Example:** `SELECT COUNT(*) FROM Employees WHERE Age > 30;`
   - **MIN() and MAX():** Returns the smallest and largest values in a column.
     - **Example:** `SELECT MIN(Salary) AS MinSalary, MAX(Salary) AS MaxSalary FROM Employees;`

6. **String Functions:**
   - **CONCAT():** Concatenates two or more strings.
     - **Example:** `SELECT CONCAT(FirstName, ' ', LastName) AS FullName FROM Employees;`
   - **SUBSTRING():** Extracts a substring from a string.
     - **Example:** `SELECT SUBSTRING(Name, 1, 3) AS SubName FROM Employees;`
   - **UPPER() and LOWER():** Converts a string to upper or lower case.
     - **Example:** `SELECT UPPER(Name) AS UpperName FROM Employees;`

7. **Date Functions:**
   - **NOW():** Returns the current date and time.
     - **Example:** `SELECT NOW() AS CurrentDateTime;`
   - **DATEDIFF():** Returns the difference in days between two dates.
     - **Example:** `SELECT DATEDIFF(NOW(), '2024-01-01') AS DaysDifference;`
   - **DATE_ADD() and DATE_SUB():** Adds or subtracts a specified time interval from a date.
     - **Example:** `SELECT DATE_ADD(NOW(), INTERVAL 10 DAY) AS FutureDate;`



Today's focus on the SQL Quick Reference Guide has provided me with a comprehensive summary of essential SQL commands and functions. This guide is incredibly useful for quick look-ups and refreshing your knowledge on key SQL concepts. As I continue this journey, I’m excited to explore more advanced SQL features and share my learnings with you.

For more detailed explanations and examples, you can check out the [W3Schools SQL Quick Reference Guide](https://www.w3schools.com/sql/sql_quickref.asp).

