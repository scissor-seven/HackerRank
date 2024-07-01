#hackerrank #SQL #silver_star-3 #population 

[Average Population of Each Continent | HackerRank](https://www.hackerrank.com/challenges/average-population-of-each-continent/problem?isFullScreen=true)

Given the **CITY** and **COUNTRY** tables, query the names of all the continents (_COUNTRY.Continent_) and their respective average city populations (_CITY.Population_) rounded _down_ to the nearest integer.
**Note:** _CITY.CountryCode_ and _COUNTRY.Code_ are matching key columns.

**Input Format**
The **CITY** and **COUNTRY** tables are described as follows:
![[Pasted image 20240613102447.png]]
![[Pasted image 20240613102454.png]]
THE QUERY:
```sql

SELECT COUNTRY.CONTINENT, FLOOR(AVG(CITY.POPULATION))
FROM CITY
INNER JOIN COUNTRY
ON CITY.COUNTRYCODE=COUNTRY.CODE
GROUP BY COUNTRY.CONTINENT;
```

1. **`SELECT COUNTRY.CONTINENT, FLOOR(AVG(CITY.POPULATION))`**:
    
    - This part of the query specifies the columns to be selected.
    - `COUNTRY.CONTINENT` selects the `CONTINENT` column from the `COUNTRY` table.
    - `FLOOR(AVG(CITY.POPULATION))` calculates the average population of cities for each continent, and `FLOOR` rounds this average down to the nearest whole number.
2. **`FROM CITY`**:
    
    - This indicates that the main table from which data is being queried is `CITY`.
3. **`INNER JOIN COUNTRY ON CITY.COUNTRYCODE = COUNTRY.CODE`**:
    
    - This performs an inner join between the `CITY` and `COUNTRY` tables.
    - The `ON` clause specifies the condition for the join: `CITY.COUNTRYCODE = COUNTRY.CODE`.
    - This means that each row in the `CITY` table is matched with a row in the `COUNTRY` table where the `COUNTRYCODE` in the `CITY` table matches the `CODE` in the `COUNTRY` table.
4. **`GROUP BY COUNTRY.CONTINENT`**:
    
    - This groups the results by the `CONTINENT` column from the `COUNTRY` table.
    - Grouping is necessary because we are using an aggregate function (`AVG`) on the `POPULATION` column. It means that the average population will be calculated for each group of cities belonging to the same continent.