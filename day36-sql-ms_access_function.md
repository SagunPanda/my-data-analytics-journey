**Day 36: Exploring SQL – MS Access Functions**

 On Day 36, I delved into MS Access functions, which are essential for performing a variety of operations within Microsoft Access databases. Understanding these functions is crucial for efficient data management and manipulation. Let's dive into some commonly used MS Access functions with simple explanations.

**Commonly Used MS Access Functions:**

1. **LEN():**
   - Returns the length of a string.
   - **Example:** `SELECT LEN(FirstName) AS Length FROM Employees;`

2. **MID():**
   - Extracts a substring from a string starting at a specified position.
   - **Example:** `SELECT MID(FirstName, 2, 3) AS Substring FROM Employees;`

3. **LEFT() and RIGHT():**
   - Returns a specified number of characters from the left (LEFT) or right (RIGHT) side of a string.
   - **Example:** `SELECT LEFT(FirstName, 2) AS LeftPart FROM Employees;`
   - **Example:** `SELECT RIGHT(FirstName, 2) AS RightPart FROM Employees;`

4. **INSTR():**
   - Returns the position of the first occurrence of a substring in a string.
   - **Example:** `SELECT INSTR(FirstName, 'a') AS Position FROM Employees;`

5. **UCASE() and LCASE():**
   - Converts a string to uppercase (UCASE) or lowercase (LCASE).
   - **Example:** `SELECT UCASE(FirstName) AS UpperCaseName FROM Employees;`
   - **Example:** `SELECT LCASE(FirstName) AS LowerCaseName FROM Employees;`

6. **DATE() and TIME():**
   - Returns the current date (DATE) or time (TIME).
   - **Example:** `SELECT DATE() AS CurrentDate;`
   - **Example:** `SELECT TIME() AS CurrentTime;`

7. **NOW():**
   - Returns the current date and time.
   - **Example:** `SELECT NOW() AS CurrentDateTime;`

8. **DATEADD():**
   - Adds a specified time interval to a date.
   - **Example:** `SELECT DATEADD('d', 5, [HireDate]) AS NewDate FROM Employees;`

9. **DATEDIFF():**
   - Returns the difference between two dates.
   - **Example:** `SELECT DATEDIFF('d', [HireDate], [EndDate]) AS DateDifference FROM Employees;`

10. **FORMAT():**
    - Formats a date or number as a string.
    - **Example:** `SELECT FORMAT([HireDate], 'yyyy-mm-dd') AS FormattedDate FROM Employees;`

11. **IIF():**
    - Performs a conditional test and returns one value if true and another if false.
    - **Example:** `SELECT IIF([Score] >= 60, 'Pass', 'Fail') AS Result FROM Students;`

12. **ISNULL():**
    - Checks if an expression is null.
    - **Example:** `SELECT ISNULL([MiddleName]) AS IsNull FROM Employees;`


Today's focus on MS Access functions has provided me with a deeper understanding of how to perform various operations within Microsoft Access databases effectively. Mastering these functions is crucial for efficient data management and manipulation. As I continue this journey, I’m excited to explore more advanced SQL features and share my learnings with you.

