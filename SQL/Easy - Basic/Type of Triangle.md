#hackerrank #SQL #silver_star-3 #triangle 

[Type of Triangle | HackerRank](https://www.hackerrank.com/challenges/what-type-of-triangle/problem?isFullScreen=true)

Write a query identifying the _type_ of each record in the **TRIANGLES** table using its three side lengths. Output one of the following statements for each record in the table:

- **Equilateral**: It's a triangle with `3` sides of equal length.
- **Isosceles**: It's a triangle with `2` sides of equal length.
- **Scalene**: It's a triangle with `3` sides of differing lengths.
- **Not A Triangle**: The given values of _A_, _B_, and _C_ don't form a triangle.

**Input Format**
The **TRIANGLES** table is described as follows:
![[Pasted image 20240613133253.png]]
Each row in the table denotes the lengths of each of a triangle's three sides.

THE QUERY :
```sql

SELECT 
	CASE
	    WHEN A + B <= C OR A + C <= B OR B + C <= A THEN 'Not A Triangle'
	    WHEN A = B AND B = C THEN 'Equilateral'
	    WHEN A = B OR B = C OR C = A THEN 'Isosceles'
	    ELSE 'Scalene'
	END AS TYPE
FROM TRIANGLES;
```

`CASE` is an **expression** that allows you to ***perform conditional logic within a query.*** It's often used to create custom categories or apply different logic based on certain conditions. The `CASE` expression is structured with `WHEN`, `THEN`, `ELSE`, and optionally `END`.

With an explanation of `CASE`, rest is pretty much clear I assume!