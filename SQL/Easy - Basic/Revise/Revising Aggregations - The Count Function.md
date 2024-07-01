#hackerrank #SQL #silver_star-3 #revise
[Revising Aggregations - The Count Function | HackerRank](https://www.hackerrank.com/challenges/revising-aggregations-the-count-function/problem?isFullScreen=true)

Query a _count_ of the number of cities in **CITY** having a _Population_ larger than `100,000`.

**Input Format**
The **CITY** table is described as follows:
![[Pasted image 20240613114323.png]]
THE QUERY :
```sql

SELECT COUNT(DISTINCT NAME) FROM CITY WHERE POPULATION>100000;
```