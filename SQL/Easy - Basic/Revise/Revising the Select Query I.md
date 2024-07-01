#hackerrank #SQL #silver_star-3 #revise 

[Revising the Select Query I | HackerRank](https://www.hackerrank.com/challenges/revising-the-select-query/problem?isFullScreen=true)

Query all columns for all American cities in the **CITY** table with populations larger than `100000`. The **CountryCode** for America is `USA`.
The **CITY** table is described as follows:
![[Pasted image 20240602203708.png]] 

THE QUERY
```sql

SELECT * FROM CITY
WHERE POPULATION>100000 AND COUNTRYCODE='USA';
```
