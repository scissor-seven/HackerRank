#hackerrank #SQL #silver_star-4 
[African Cities | HackerRank](https://www.hackerrank.com/challenges/african-cities/problem?isFullScreen=true)

Given the **CITY** and **COUNTRY** tables, query the names of all cities where the _CONTINENT_ is _'Africa'_.
**Note:** _CITY.CountryCode_ and _COUNTRY.Code_ are matching key columns.

**Input Format**
The **CITY** and **COUNTRY** tables are described as follows:
![[Pasted image 20240613134232.png]]
![[Pasted image 20240613134240.png]]
THE QUERY :
```sql

SELECT CITY.NAME FROM CITY
JOIN COUNTRY
ON CITY.COUNTRYCODE = COUNTRY.CODE
WHERE COUNTRY.CONTINENT='AFRICA';
```

The query is pretty understood if you are coming here from [[Avg Population of Each Continent]] problem. Very similar, but not as complicated as that one.