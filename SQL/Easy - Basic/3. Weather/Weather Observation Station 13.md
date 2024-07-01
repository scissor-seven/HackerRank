#hackerrank #SQL #bronze_star #regex 

[Weather Observation Station 13 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-13/problem?isFullScreen=true)

Query the sum of _Northern Latitudes_ (_LAT_N_) from **STATION** having values greater than `38.7880` and less than `137.2345`. Truncate your answer to  decimal places.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240604182344.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.
THE QUERY:
```sql

SELECT ROUND(SUM(LAT_N), 4) FROM STATION WHERE LAT_N BETWEEN 38.7880 AND 137.2345;
```
2 main things to consider in this query:
- `ROUND(SUM(LAT_N), 4)`: *This part of query does the main thing, which is to first sum up the lat_n values, then round 'em up to 4 decimal places using round where first argument is the sum from before, and second is no. decimal of decimal places!*
- `BETWEEN` keyword, which is used here, is **one of the keywords** *used to provide the query with a range of selection*. **Syntax is pretty clear**!

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-12/problem?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 12]]
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-14?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 14]].

For more info on regex, consider reading [[Regular Expression Pattern]].