#hackerrank #SQL #silver_star-3 #employee 

[The Blunder | HackerRank](https://www.hackerrank.com/challenges/the-blunder/problem?isFullScreen=true)

Samantha was tasked with calculating the average monthly salaries for all employees in the **EMPLOYEES** table, but did not realize her keyboard's  key was broken until after completing the calculation. She wants your help finding the difference between her miscalculation (using salaries with any zeros removed), and the actual average salary.

Write a query calculating the amount of error (i.e.:  average monthly salaries), and round it up to the next integer.

**Input Format**
The **EMPLOYEES** table is described as follows:
![[Pasted image 20240613112254.png]]
**Note:** _Salary_ is per month.

THE QUERY :
```sql

SELECT CEIL(AVG(SALARY)- AVG(REPLACE(SALARY, 0 , "")))
FROM EMPLOYEES;
```

I think the expression might need some explanation...
1. **`REPLACE(SALARY, 0, '')`**:
	- The `REPLACE` function takes three arguments: the column to operate on, the string to find, and the string to replace it with.
	- In this case, it replaces all occurrences of the digit '0' in the `SALARY` column with an empty string `''`.
	- For example, if `SALARY` is `2000`, the `REPLACE(SALARY, 0, '')` would result in `2`.

2. **`CEIL(...)`**:
	- The `CEIL` (ceiling) function rounds the result up to the nearest integer.