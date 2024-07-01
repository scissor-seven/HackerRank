#hackerrank #SQL #bronze_star 

[Weather Observation Station 3 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-3/problem?isFullScreen=true)

Query a list of **CITY** names from **STATION** for cities that have an even **ID** number. Print the results in any order, but exclude duplicates from the answer.  
The **STATION** table is described as follows:
![[Pasted image 20240603123555.png]]
where **LAT_N** is the northern latitude and **LONG_W** is the western longitude.

THE QUERY:
```SQL

SELECT DISTINCT(CITY) FROM STATION WHERE ID%2=0;
```
EXPLANATION:
- Once again, only 2 things new, `DISTINCT()` & **WHERE** clause.
- `DISTINCT()` this function **prohibits selection of duplicate data**, like, in cases where duplicate data is needed to be excluded, this function is used.
- `ID%2=0`, read as `ID modulo 2 equals 0` (I mean, that's how I read, at least 🤷🏻), is an **expression** to *check if data in ID is even or not*. `%` this operator checks whether the remainder after division is `zero` or not! *I mean, isn't that how we check for an even number!*

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-2?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 2]]
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-4?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 4]].