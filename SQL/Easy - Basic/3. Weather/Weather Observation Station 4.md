#hackerrank #SQL #bronze_star 

[Weather Observation Station 4 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-4/problem?isFullScreen=true)

Find the difference between the total number of **CITY** entries in the table and the number of distinct **CITY** entries in the table.  
The **STATION** table is described as follows:
![[Pasted image 20240603130312.png]]
where **LAT_N** is the northern latitude and **LONG_W** is the western longitude.

For example, if there are three records in the table with **CITY** values 'New York', 'New York', 'Bengaluru', there are 2 different city names: 'New York' and 'Bengaluru'. The query returns 1 , because
`total no. of records - no. of unique city names = 3 - 2 = 1`.

THE QUERY:
```SQL

SELECT COUNT(CITY) - COUNT(DISTINCT(CITY)) FROM STATION;
```
EXPLANATION:
- A new function `COUNT()` is introduced, which basically *counts no. of records for a column.*
- Rest is either pretty standard or explained previously.

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-3?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 3]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-5?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 5]].