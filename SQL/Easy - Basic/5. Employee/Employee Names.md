#hackerrank #SQL #silver_star-3 #employee

[Employee Names | HackerRank](https://www.hackerrank.com/challenges/name-of-employees/problem?isFullScreen=true)

Write a query that prints a list of employee names (i.e.: the _name_ attribute) from the **Employee** table in alphabetical order.

**Input Format**
The **Employee** table containing employee data for a company is described as follows:
![[Pasted image 20240613105346.png]]
where _employee_id_ is an employee's ID number, _name_ is their name, _months_ is the total number of months they've been working for the company, and _salary_ is their monthly salary.

THE QUERY:
```sql

SELECT NAME FROM EMPLOYEE ORDER BY NAME ASC;
```
- Pretty straight forward if you ask me.