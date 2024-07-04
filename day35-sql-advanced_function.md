**Day 35: Exploring SQL – Advanced Functions**

 On Day 35, I delved into advanced SQL functions, which are powerful tools for performing complex operations on data. Understanding these functions is crucial for sophisticated data analysis and manipulation. Let's dive into some commonly used advanced SQL functions with simple explanations.

**Commonly Used Advanced SQL Functions:**

1. **COALESCE():**
   - Returns the first non-null value in a list of expressions.
   - **Example:** `SELECT COALESCE(NULL, 'default', 'value') AS Result;`

2. **NULLIF():**
   - Returns NULL if the two expressions are equal, otherwise returns the first expression.
   - **Example:** `SELECT NULLIF(10, 10) AS Result;`

3. **CASE:**
   - Evaluates a list of conditions and returns one of multiple possible result expressions.
   - **Example:** 
     ```
     SELECT 
       CASE 
         WHEN score >= 90 THEN 'A' 
         WHEN score >= 80 THEN 'B' 
         ELSE 'C' 
       END AS Grade 
     FROM Students;
     ```

4. **CAST() and CONVERT():**
   - Converts an expression from one data type to another.
   - **Example:** `SELECT CAST('2024-06-26' AS DATE) AS DateValue;`
   - **Example:** `SELECT CONVERT(DATE, '2024-06-26') AS DateValue;`

5. **IFNULL():**
   - Returns a specified value if the expression is NULL.
   - **Example:** `SELECT IFNULL(NULL, 'default') AS Result;`

6. **ISNULL():**
   - Checks if an expression is NULL.
   - **Example:** `SELECT ISNULL(NULL) AS Result;`

7. **LEAD() and LAG():**
   - Provides access to a row at a given physical offset that comes after (LEAD) or before (LAG) the current row.
   - **Example:** `SELECT LEAD(salary, 1) OVER (ORDER BY id) AS NextSalary FROM Employees;`
   - **Example:** `SELECT LAG(salary, 1) OVER (ORDER BY id) AS PreviousSalary FROM Employees;`

8. **ROW_NUMBER():**
   - Assigns a unique number to each row according to the specified ordering.
   - **Example:** `SELECT ROW_NUMBER() OVER (ORDER BY salary DESC) AS RowNum, * FROM Employees;`

9. **RANK() and DENSE_RANK():**
   - Assigns a rank to each row within the partition of a result set.
   - **Example:** `SELECT RANK() OVER (ORDER BY salary DESC) AS Rank, * FROM Employees;`
   - **Example:** `SELECT DENSE_RANK() OVER (ORDER BY salary DESC) AS DenseRank, * FROM Employees;`

10. **NTILE():**
    - Divides the result set into a specified number of roughly equal parts.
    - **Example:** `SELECT NTILE(4) OVER (ORDER BY salary DESC) AS Quartile, * FROM Employees;`


Today's focus on advanced SQL functions has provided me with a deeper understanding of how to perform sophisticated operations on data effectively. Mastering these functions is crucial for advanced data analysis and manipulation. As I continue this journey, I’m excited to explore more complex SQL features and share my learnings with you.

