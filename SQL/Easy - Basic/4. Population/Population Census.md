#hackerrank #SQL #silver_star-3 #population 

[Population Census | HackerRank](https://www.hackerrank.com/challenges/asian-population/problem?isFullScreen=true)

 Given the **CITY** and **COUNTRY** tables, query the sum of the populations of all cities where the _CONTINENT_ is _'Asia'_.
**Note:** _CITY.CountryCode_ and _COUNTRY.Code_ are matching key columns.

**Input Format**
The **CITY** and **COUNTRY** tables are described as follows:
![[Pasted image 20240613002002.png]]
![[Pasted image 20240613002009.png]]
THE QUERY:
```sql

SELECT SUM(CITY.POPULATION)
FROM CITY JOIN COUNTRY
ON CITY.COUNTRYCODE=CODE
WHERE COUNTRY.CONTINENT='ASIA';
```
- Join `CITY` and `COUNTRY` on `CITY.COUNTRYCODE = COUNTRY.CODE`.
- Filter to include only rows where `COUNTRY.CONTINENT = 'Asia'`.
- Sum the `POPULATION` of the cities in these filtered rows.

Although explained above, I think this needs a bit detailed explanation than just that!

1. **`SELECT SUM(CITY.POPULATION)`**:
    - This part of the query specifies that you want to calculate the sum of the population of cities.
    - `SUM(CITY.POPULATION)` aggregates the population values from the `CITY` table.

2. **`FROM CITY`**: 
    - This indicates that the main table you're querying data from is `CITY`.

3. **`JOIN COUNTRY ON CITY.COUNTRYCODE = COUNTRY.CODE`**: 
    - This performs an inner join between the `CITY` and `COUNTRY` tables.
    - The `ON` clause specifies the condition for the join: `CITY.COUNTRYCODE = COUNTRY.CODE`.
    - `CITY.COUNTRYCODE` is a foreign key in the `CITY` table that references the `CODE` primary key in the `COUNTRY` table.
    - This join ensures that each city is paired with its corresponding country based on the matching country code.

4. **`WHERE COUNTRY.CONTINENT = 'ASIA'`**: 
    - This filters the results to include only the rows where the `CONTINENT` column in the `COUNTRY` table is equal to 'ASIA'.
    - This means that only the cities located in countries that are part of the continent 'Asia' are considered in the result.