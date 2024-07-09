**Day 38: Practicing SQL Queries**

On Day 38, I dedicated my time to practicing various SQL queries. This hands-on practice is crucial for reinforcing the concepts and commands I've learned so far. Here's a recap of some of the queries I worked on, highlighting different aspects of SQL.

**SQL Query Practice:**

1. **Basic Select Queries:**
   - **Example:** Retrieve all records from the Employees table.
     - `SELECT * FROM Employees;`

2. **Filtering Data with WHERE:**
   - **Example:** Get employees older than 30.
     - `SELECT * FROM Employees WHERE Age > 30;`

3. **Sorting Data with ORDER BY:**
   - **Example:** List employees by salary in descending order.
     - `SELECT * FROM Employees ORDER BY Salary DESC;`

4. **Using Aggregate Functions:**
   - **Example:** Calculate the average salary of employees.
     - `SELECT AVG(Salary) AS AverageSalary FROM Employees;`
   - **Example:** Count the number of employees in each department.
     - `SELECT Department, COUNT(*) AS EmployeeCount FROM Employees GROUP BY Department;`

5. **Joining Tables:**
   - **Example:** Combine employee and department information.
     - `SELECT Employees.Name, Departments.Department FROM Employees INNER JOIN Departments ON Employees.DepartmentID = Departments.ID;`

6. **Using String Functions:**
   - **Example:** Concatenate first and last names.
     - `SELECT CONCAT(FirstName, ' ', LastName) AS FullName FROM Employees;`

7. **Date Functions:**
   - **Example:** Find employees hired in the last year.
     - `SELECT * FROM Employees WHERE HireDate >= DATE_SUB(NOW(), INTERVAL 1 YEAR);`

8. **Subqueries:**
   - **Example:** Find the employee with the highest salary.
     - `SELECT * FROM Employees WHERE Salary = (SELECT MAX(Salary) FROM Employees);`

9. **Using CASE Statements:**
   - **Example:** Categorize employees based on their age.
     ```
     SELECT Name, 
       CASE 
         WHEN Age < 30 THEN 'Young' 
         WHEN Age BETWEEN 30 AND 50 THEN 'Middle-aged' 
         ELSE 'Senior' 
       END AS AgeCategory 
     FROM Employees;
     ```

10. **Updating Data:**
    - **Example:** Give a 10% raise to employees in the Sales department.
      - `UPDATE Employees SET Salary = Salary * 1.10 WHERE DepartmentID = (SELECT ID FROM Departments WHERE Department = 'Sales');`

11. **Deleting Data:**
    - **Example:** Remove employees who have left the company.
      - `DELETE FROM Employees WHERE Status = 'Left';`

12. **Using Views:**
    - **Example:** Create a view for active employees.
      - `CREATE VIEW ActiveEmployees AS SELECT * FROM Employees WHERE Status = 'Active';`



Today's practice session was incredibly productive. Working through these queries has solidified my understanding of SQL and prepared me for more advanced topics. Hands-on practice is key to mastering SQL, and I’m excited to continue improving my skills.
