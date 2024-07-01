#hackerrank #SQL #silver_star-3 #employee

[Employee Salaries | HackerRank](https://www.hackerrank.com/challenges/salary-of-employees/problem?isFullScreen=true)

Write a query that prints a list of employee names (i.e.: the _name_ attribute) for employees in **Employee** having a salary greater than  per month who have been employees for less than  months. Sort your result by ascending _employee_id_.

**Input Format**
The **Employee** table containing employee data for a company is described as follows:
![[Pasted image 20240613110052.png]]
where _employee_id_ is an employee's ID number, _name_ is their name, _months_ is the total number of months they've been working for the company, and _salary_ is the their monthly salary.

THE QUERY:
```sql

SELECT NAME FROM EMPLOYEE WHERE SALARY>2000 AND MONTHS<10;
```
- Once again, we got this! Done harder stuff than this before