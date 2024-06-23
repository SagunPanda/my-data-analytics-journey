**Day 26: Exploring SQL – Constraints**

 On Day 26, I delved into SQL constraints, which are rules enforced on data columns in a table. Constraints are crucial for maintaining data integrity and ensuring the accuracy and reliability of the data in the database. Let's dive into each type of constraint with simple examples explained in text.

**Types of SQL Constraints:**

1. **NOT NULL:**
   - Ensures that a column cannot have a NULL value.
   - **Example:** To make sure that every employee has an `EmployeeID`, you would apply the NOT NULL constraint to the `EmployeeID` column.

2. **UNIQUE:**
   - Ensures that all values in a column are different.
   - **Example:** To ensure that each email address in the `Employees` table is unique, you would apply the UNIQUE constraint to the `Email` column.

3. **PRIMARY KEY:**
   - Uniquely identifies each record in a table. It must contain unique values and cannot contain NULL values.
   - **Example:** To uniquely identify each employee, you would set the `EmployeeID` column as the PRIMARY KEY.

4. **FOREIGN KEY:**
   - Ensures referential integrity by linking two tables. It matches the value in one table to the primary key in another table.
   - **Example:** To link employees to their departments, you would use a FOREIGN KEY constraint on the `DepartmentID` column in the `Employees` table, referencing the `DepartmentID` column in the `Departments` table.

5. **CHECK:**
   - Ensures that all values in a column satisfy a specific condition.
   - **Example:** To ensure that employees' ages are 18 or older, you would apply a CHECK constraint to the `Age` column.

6. **DEFAULT:**
   - Sets a default value for a column if no value is specified.
   - **Example:** To set the default department to 'General' if no department is assigned, you would apply the DEFAULT constraint to the `Department` column.
