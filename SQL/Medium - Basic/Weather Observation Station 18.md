#hackerrank #silver_star-4 #SQL #medium #basic 

[Weather Observation Station 18 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-18/problem?isFullScreen=true)

This wasn't a very complicated question to begin with, but there are various things one can learn from it, if they try multiple ways to solve this query.

Here's one way:
- If you look at the query in an expanded format, you won't see anything that we haven't used up to this point. Just a regular `ROUND` function with `MIN` and `MAX` within it on `LAT_N` and `LONG_W`.
```sql

SELECT ROUND(MAX(LAT_N)-MIN(LAT_N) + MAX(LONG_W)-MIN(LONG_W), 4)
FROM STATION;
```
Here's what I used:
- This query utilizes a new function (not new technically) `ABS` which means *absolute* which is *basically a **mathematical mod** in **SQL** format*.
- The way I wrote the distance expression didn't technically need the `ABS` function, but there can be times, when records can all get negative, even when they are not supposed to, this is for that!
```sql

SELECT ROUND(ABS(MAX(LAT_N)-MIN(LAT_N)) + ABS(MAX(LONG_W)-MIN(LONG_W)), 4)
AS ManhattanDistance
FROM STATION;
```

If you have any other way that you used, as simple as possible, do put them on them on twitter or any other platform and tag me!

[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-19?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 19]].