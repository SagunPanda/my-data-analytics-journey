**Day 34: Exploring SQL – Date Functions**

 On Day 34, I explored SQL date functions, which are essential for manipulating and extracting information from date and time data. Understanding these functions is crucial for performing operations involving dates and times. Let's dive into some commonly used SQL date functions with simple explanations.

**Commonly Used SQL Date Functions:**

1. **CURRENT_DATE():**
   - Returns the current date.
   - **Example:** `SELECT CURRENT_DATE() AS CurrentDate;`

2. **CURRENT_TIME():**
   - Returns the current time.
   - **Example:** `SELECT CURRENT_TIME() AS CurrentTime;`

3. **CURRENT_TIMESTAMP():**
   - Returns the current date and time.
   - **Example:** `SELECT CURRENT_TIMESTAMP() AS CurrentTimestamp;`

4. **DATE():**
   - Extracts the date part of a date or datetime expression.
   - **Example:** `SELECT DATE('2024-06-26 12:34:56') AS DatePart;`

5. **DATE_ADD():**
   - Adds a specified time interval to a date.
   - **Example:** `SELECT DATE_ADD('2024-06-26', INTERVAL 5 DAY) AS NewDate;`

6. **DATE_SUB():**
   - Subtracts a specified time interval from a date.
   - **Example:** `SELECT DATE_SUB('2024-06-26', INTERVAL 5 DAY) AS NewDate;`

7. **DATEDIFF():**
   - Returns the number of days between two dates.
   - **Example:** `SELECT DATEDIFF('2024-06-26', '2024-06-21') AS DateDifference;`

8. **EXTRACT():**
   - Extracts a part of a date.
   - **Example:** `SELECT EXTRACT(YEAR FROM '2024-06-26') AS YearPart;`

9. **STR_TO_DATE():**
   - Converts a string to a date.
   - **Example:** `SELECT STR_TO_DATE('26-06-2024', '%d-%m-%Y') AS DateValue;`

10. **TIME():**
    - Extracts the time part of a date or datetime expression.
    - **Example:** `SELECT TIME('2024-06-26 12:34:56') AS TimePart;`

11. **TIMESTAMP():**
    - Returns a datetime value based on date or datetime parts.
    - **Example:** `SELECT TIMESTAMP('2024-06-26', '12:34:56') AS DateTimeValue;`

12. **YEAR(), MONTH(), DAY():**
    - Extracts the year, month, or day from a date.
    - **Example:** `SELECT YEAR('2024-06-26') AS YearPart, MONTH('2024-06-26') AS MonthPart, DAY('2024-06-26') AS DayPart;`


Today's focus on SQL date functions has provided me with a deeper understanding of how to manipulate and extract information from date and time data effectively. Mastering these functions is crucial for performing operations involving dates and times. As I continue this journey, I’m excited to explore more advanced SQL features and share my learnings with you.
