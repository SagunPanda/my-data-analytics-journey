**Day 21: Exploring SQL – UNION, GROUP BY, HAVING, EXISTS**

On Day 21, I delved into some more advanced SQL commands: UNION, GROUP BY, HAVING, and EXISTS. These commands are essential for combining query results, grouping data, filtering grouped data, and checking for the existence of records. Let's dive into each of these concepts with simple examples explained in text.

**UNION Statement:**

The `UNION` statement is used to combine the result sets of two or more SELECT statements. Each SELECT statement within the UNION must have the same number of columns in the result sets with similar data types.

- **Example:** To combine the lists of employees from two different departments, you would use UNION to merge these lists into a single result set.

**GROUP BY Statement:**

The `GROUP BY` statement is used to arrange identical data into groups.

- **Example:** To find the total salary paid in each department, you would use GROUP BY to group the records by department and then calculate the total salary for each group.

**HAVING Clause:**

The `HAVING` clause is used to filter groups based on a specified condition, similar to how the WHERE clause filters rows.

- **Example:** To find departments with a total salary expense greater than 100,000, you would use GROUP BY to group the records by department, then use HAVING to filter those groups based on the total salary condition.

**EXISTS Operator:**

The `EXISTS` operator is used to test for the existence of any record in a subquery. It returns true if the subquery returns one or more records.

- **Example:** To find employees who belong to a department that has more than five employees, you would use EXISTS to check for the existence of such departments and then filter employees based on that condition.


Today's exploration of advanced SQL commands has been highly enriching. Understanding how to use UNION, GROUP BY, HAVING, and EXISTS is crucial for performing complex queries and data analysis. As I continue this journey, I’m excited to explore more SQL features and share my learnings with you.

