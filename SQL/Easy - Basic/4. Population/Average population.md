#hackerrank #SQL #silver_star-3 #population

[Average Population | HackerRank](https://www.hackerrank.com/challenges/average-population/problem?isFullScreen=true)

Query the average population for all cities in **CITY**, rounded _down_ to the nearest integer.
**Input Format**
The **CITY** table is described as follows:
![[Pasted image 20240613000302.png]]
THE QUERY:
```sql

SELECT ROUND(AVG(POPULATION), 0) FROM CITY;
```
- Once again, pretty standard functions, `avg()` for averaging round to make it into closest integer.