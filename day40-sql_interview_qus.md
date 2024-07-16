**Title: Day 40: Practicing SQL Interview Questions**


 On Day 40, I focused on practicing SQL interview questions. This preparation is crucial for job interviews, as it tests not only theoretical knowledge but also practical problem-solving skills. Here's a summary of the types of questions I tackled and the concepts they covered.

**SQL Interview Questions Practice:**

1. **Basic Queries:**
   - **Question:** Retrieve the names of all employees.
     - `SELECT Name FROM Employees;`
   - **Question:** Count the total number of employees.
     - `SELECT COUNT(*) FROM Employees;`

2. **Filtering Data:**
   - **Question:** Get all employees who are older than 30.
     - `SELECT * FROM Employees WHERE Age > 30;`
   - **Question:** Find employees in the IT department.
     - `SELECT * FROM Employees WHERE Department = 'IT';`

3. **Sorting and Grouping:**
   - **Question:** List employees by salary in descending order.
     - `SELECT * FROM Employees ORDER BY Salary DESC;`
   - **Question:** Group employees by department and count them.
     - `SELECT Department, COUNT(*) FROM Employees GROUP BY Department;`

4. **Joins:**
   - **Question:** Combine employee information with their department names.
     - `SELECT Employees.Name, Departments.Department FROM Employees INNER JOIN Departments ON Employees.DepartmentID = Departments.ID;`
   - **Question:** List all employees along with their manager's name.
     - `SELECT E.Name AS Employee, M.Name AS Manager FROM Employees E LEFT JOIN Employees M ON E.ManagerID = M.ID;`

5. **Aggregate Functions:**
   - **Question:** Calculate the average salary of all employees.
     - `SELECT AVG(Salary) AS AverageSalary FROM Employees;`
   - **Question:** Find the department with the highest total salary.
     - `SELECT Department, SUM(Salary) AS TotalSalary FROM Employees GROUP BY Department ORDER BY TotalSalary DESC LIMIT 1;`

6. **Subqueries:**
   - **Question:** Find the employee with the second highest salary.
     - `SELECT Name, Salary FROM Employees WHERE Salary = (SELECT MAX(Salary) FROM Employees WHERE Salary < (SELECT MAX(Salary) FROM Employees));`
   - **Question:** List employees who have a higher salary than the average salary.
     - `SELECT Name, Salary FROM Employees WHERE Salary > (SELECT AVG(Salary) FROM Employees);`

7. **String Functions:**
   - **Question:** Get the first three letters of each employee's name.
     - `SELECT SUBSTRING(Name, 1, 3) AS ShortName FROM Employees;`
   - **Question:** Concatenate first name and last name of employees.
     - `SELECT CONCAT(FirstName, ' ', LastName) AS FullName FROM Employees;`

8. **Date Functions:**
   - **Question:** Find employees who joined in the last six months.
     - `SELECT * FROM Employees WHERE HireDate >= DATE_SUB(CURDATE(), INTERVAL 6 MONTH);`
   - **Question:** Calculate the tenure of each employee.
     - `SELECT Name, DATEDIFF(CURDATE(), HireDate) AS TenureDays FROM Employees;`

9. **Advanced Queries:**
   - **Question:** Find duplicate records in the Employees table.
     - `SELECT Name, COUNT(*) FROM Employees GROUP BY Name HAVING COUNT(*) > 1;`
   - **Question:** Delete employees who have left the company.
     - `DELETE FROM Employees WHERE Status = 'Left';`

10. **Performance Optimization:**
    - **Question:** Optimize a query that retrieves all active employees.
      - Ensure proper indexing and use of WHERE clauses:
      - `SELECT * FROM Employees WHERE Status = 'Active';`


Today's session was focused on preparing for SQL interview questions, which has been incredibly helpful in reinforcing my knowledge and improving my problem-solving skills. These questions cover a range of topics from basic queries to more advanced concepts, providing a comprehensive review.

