#hackerrank #SQL #bronze_star

[Weather Observation Station 14 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-14/problem?isFullScreen=true)

Query the greatest value of the _Northern Latitudes_ (_LAT_N_) from **STATION** that is less than `137.2345`. Truncate your answer to `4` decimal places.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240607120540.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.

THE QUERY:
```sql

SELECT ROUND(MAX(LAT_N), 4) FROM STATION WHERE LAT_N<137.2345;
```
- I think it it pretty straight-forward by now, like, it pretty standard, `max()` function will take the highest record from `LAT_N` table.
- Which will then be truncated up to `4 decimal places` by `round()` function.

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-13/problem?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 13]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-15?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 15]].