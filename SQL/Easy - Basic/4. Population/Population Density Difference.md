#hackerrank #SQL #silver_star-3 #population 

[Population Density Difference | HackerRank](https://www.hackerrank.com/challenges/population-density-difference/problem?isFullScreen=true)

Query the difference between the maximum and minimum populations in **CITY**.
**Input Format**
The **CITY** table is described as follows:
![[Pasted image 20240613001602.png]]
THE QUERY:
```sql

SELECT (MAX(POPULATION)-MIN(POPULATION)) FROM CITY;
```
- Often times, we use expressions when a complicated `selection` has to be made. 

This one was not very trivial.