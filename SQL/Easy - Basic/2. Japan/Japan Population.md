#hackerrank #SQL #bronze_star #japan

[Japan Population | HackerRank](https://www.hackerrank.com/challenges/japan-population/problem?isFullScreen=true)

Query the sum of the populations for all Japanese cities in **CITY**. The _COUNTRYCODE_ for Japan is **JPN**.
**Input Format**
The **CITY** table is described as follows:
![[Pasted image 20240612235020.png]]
THE QUERY:
```SQL
SELECT SUM(POPULATION) FROM CITY WHERE COUNTRYCODE='JPN';
```
- Not much to explain here! Pretty standard `sum()` function on population field.