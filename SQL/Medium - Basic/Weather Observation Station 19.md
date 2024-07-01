#hackerrank #SQL #silver_star-4 #medium #basic 

[Weather Observation Station 19 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-19/problem?isFullScreen=true)

This like previous, not a very complicated query here just congested and squeezed with mathematical functions. If opened up, everything is pretty clear and standard.

I personally don't think this requires a need to be explained:
```sql

SELECT ROUND( SQRT( POW( MAX(LAT_N)-MIN(LAT_N), 2) + POW( MAX(LONG_W)-MIN(LONG_W ), 2) ), 4)
FROM STATION;
```
Just try to read and understand this very calmy, the more you understand by yourself, the more you'll be able to grasp the concepts and start making your own queries, right or wrong don't matter!

------------------------------------------------------------------
The `medium difficulty` `Weather Observation Station` series on `basic level` ends here!
It is continued on `Medium Difficulty, Intermediate Level` here -> [[Weather Observation Station 20]].

----------------------------------------------------------------------------------------