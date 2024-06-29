**Day 31: Exploring MySQL Functions**

 On Day 31, I delved into MySQL functions, which are essential for performing operations on data and returning a single value. Understanding these functions is crucial for data manipulation and analysis. Let's dive into some commonly used MySQL functions with simple explanations.

**Commonly Used MySQL Functions:**

1. **Aggregate Functions:**
   - **COUNT():** Returns the number of rows that match a specified condition.
     - **Example:** `SELECT COUNT(*) FROM Employees;`
   - **SUM():** Returns the total sum of a numeric column.
     - **Example:** `SELECT SUM(Salary) FROM Employees;`
   - **AVG():** Returns the average value of a numeric column.
     - **Example:** `SELECT AVG(Salary) FROM Employees;`
   - **MIN():** Returns the minimum value in a column.
     - **Example:** `SELECT MIN(Salary) FROM Employees;`
   - **MAX():** Returns the maximum value in a column.
     - **Example:** `SELECT MAX(Salary) FROM Employees;`

2. **String Functions:**
   - **CONCAT():** Concatenates two or more strings.
     - **Example:** `SELECT CONCAT(FirstName, ' ', LastName) AS FullName FROM Employees;`
   - **UPPER():** Converts a string to uppercase.
     - **Example:** `SELECT UPPER(FirstName) FROM Employees;`
   - **LOWER():** Converts a string to lowercase.
     - **Example:** `SELECT LOWER(FirstName) FROM Employees;`
   - **SUBSTRING():** Extracts a substring from a string.
     - **Example:** `SELECT SUBSTRING(FirstName, 1, 3) FROM Employees;`
   - **LENGTH():** Returns the length of a string.
     - **Example:** `SELECT LENGTH(FirstName) FROM Employees;`

3. **Date and Time Functions:**
   - **NOW():** Returns the current date and time.
     - **Example:** `SELECT NOW();`
   - **CURDATE():** Returns the current date.
     - **Example:** `SELECT CURDATE();`
   - **CURTIME():** Returns the current time.
     - **Example:** `SELECT CURTIME();`
   - **DATEDIFF():** Returns the difference in days between two dates.
     - **Example:** `SELECT DATEDIFF(NOW(), HireDate) FROM Employees;`
   - **DATE_FORMAT():** Formats a date value according to a specified format.
     - **Example:** `SELECT DATE_FORMAT(HireDate, '%Y-%m-%d') FROM Employees;`

4. **Numeric Functions:**
   - **ABS():** Returns the absolute value of a number.
     - **Example:** `SELECT ABS(-10);`
   - **ROUND():** Rounds a number to a specified number of decimal places.
     - **Example:** `SELECT ROUND(Salary, 2) FROM Employees;`
   - **CEIL():** Returns the smallest integer value greater than or equal to a number.
     - **Example:** `SELECT CEIL(Salary) FROM Employees;`
   - **FLOOR():** Returns the largest integer value less than or equal to a number.
     - **Example:** `SELECT FLOOR(Salary) FROM Employees;`
