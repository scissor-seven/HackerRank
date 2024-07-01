#hackerrank #SQL #bronze_star 

[Weather Observation Station 15 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-15/problem?isFullScreen=true)

Query the _Western Longitude_ (_LONG_W_) for the largest _Northern Latitude_ (_LAT_N_) in **STATION** that is less than `137.2345` . Round your answer to `4` decimal places.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240607123341.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.

THE QUERY:
```sql

SELECT ROUND(LONG_W, 4) FROM STATION WHERE LAT_N= (SELECT MAX(LAT_N) FROM STATION WHERE LAT_N<137.2345) ;
```
**Now THIS, is an interesting query!!!**
- I guess from start, up to `where` clause is pretty standard, but after `where` is where the magic lies!
- We make another `select query`, which was basically somewhat from previous query, and pass it on as `LAT_N`, which becomes a `where clause` filter for our preceding query. **Isn't that genius!**

And that was all for this challenge....
[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-14/problem?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 14]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-16?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 16]].