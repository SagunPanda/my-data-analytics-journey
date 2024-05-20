 Day 1: Mastering Excel Basics - SUM, MIN, MAX, RIGHT, LEFT, and SPLIT

 **SUM Function:**
 The SUM function in Excel is incredibly useful for adding up numbers in a range of cells. Whether you're summing up sales figures, expenses, or any other data, SUM makes it easy. Here's a quick example:

```
=SUM(A1:A10)
```
This formula will add up all the values from cell A1 to A10. It's straightforward but powerful when dealing with large datasets.

**MIN and MAX Functions:**

Finding the smallest and largest values in a dataset is crucial for analysis. The MIN and MAX functions do just that. For example:

```
=MIN(B1:B10)
=MAX(B1:B10)
```

These formulas will return the smallest and largest values in the range B1 to B10, respectively. These functions are great for quickly identifying the range of your data.

**RIGHT and LEFT Functions:**

Sometimes, you need to extract specific parts of a text string. The RIGHT and LEFT functions help you do this. For instance:

```
=RIGHT(C1, 5)
=LEFT(C1, 3)
```

The RIGHT function extracts the last 5 characters from the text in cell C1, while the LEFT function extracts the first 3 characters. These are handy for working with text data where you need specific segments.

**SPLIT Function:**

In Excel, the SPLIT function isn't directly available, but you can achieve similar results using the Text to Columns feature or combinations of other functions like FIND and MID. Here's how you can split a full name into first and last names:

1. **Text to Columns:**
   - Select the column with the text you want to split.
   - Go to the Data tab and click Text to Columns.
   - Choose Delimited and click Next.
   - Select the delimiter (e.g., space) and click Finish.

2. **Using FIND and MID:**
   ```
   First Name: =LEFT(D1, FIND(" ", D1) - 1)
   Last Name: =MID(D1, FIND(" ", D1) + 1, LEN(D1))
   ```

   These formulas assume the first space separates the first and last names in cell D1.
