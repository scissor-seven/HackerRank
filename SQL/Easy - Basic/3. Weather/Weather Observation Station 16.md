#hackerrank #SQL #bronze_star 

[Weather Observation Station 16 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-16/problem?isFullScreen=true)

Query the smallest _Northern Latitude_ (_LAT_N_) from **STATION** that is greater than `38.7780`. Round your answer to `4` decimal places.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240607124004.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.

THE QUERY:
```sql

SELECT ROUND(MIN(LAT_N), 4) FROM STATION WHERE LAT_N>38.7780;
```
- **What!? You want explanation for this, get outta here man!**

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-15/problem?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 15]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-17?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 17]].